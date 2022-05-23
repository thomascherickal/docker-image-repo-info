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
-	[`nats:2.8.3`](#nats283)
-	[`nats:2.8.3-alpine`](#nats283-alpine)
-	[`nats:2.8.3-alpine3.15`](#nats283-alpine315)
-	[`nats:2.8.3-linux`](#nats283-linux)
-	[`nats:2.8.3-nanoserver`](#nats283-nanoserver)
-	[`nats:2.8.3-nanoserver-1809`](#nats283-nanoserver-1809)
-	[`nats:2.8.3-scratch`](#nats283-scratch)
-	[`nats:2.8.3-windowsservercore`](#nats283-windowsservercore)
-	[`nats:2.8.3-windowsservercore-1809`](#nats283-windowsservercore-1809)
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
$ docker pull nats@sha256:faf79ebeddcf0d20856df247744cdf519e8051a2480cb12b9f53c4c2e0086b3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2928; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:c4c5aa8d8b2ce861febd7bd4dcd9a729204ba3f15f91fd96f45ab5a6e100e516
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4590377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ca6ed6836bb8a2f8705608091864ce3c25b8ca32693003e2a8df04e30dc0f9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:19:51 GMT
COPY file:8ff89c4fbf2c06b0c443f547e21c09f4d00bc37565795d87bfb43a04d4ff236e in /nats-server 
# Mon, 23 May 2022 22:19:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:19:51 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:19:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:19:52 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:19:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:49229864ce5450b6b5291aa946e418a9b56e6bbac1179c2a3ca592284b674f6c`  
		Last Modified: Mon, 23 May 2022 22:20:42 GMT  
		Size: 4.6 MB (4589871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f11a75312c73ef42e06951cc5acd4b2690648b1ab001bacda9622a11819993`  
		Last Modified: Mon, 23 May 2022 22:20:41 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:0a83bd61fe2f1ebbf052ab13bd453c3dfaec1db3e86896718024aff558174bf9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea45afb007d73aa5822eb21ef9e9d34b90edd8cbb44379c26a50b550889c3d3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 23:13:43 GMT
COPY file:4121ba71c4705779a334ba22404be19aaa6e3e8946ec6b5ce733466627f8c88e in /nats-server 
# Mon, 23 May 2022 23:13:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 23:13:44 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 23:13:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 23:13:45 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 23:13:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3429a8151ae5ab692b14a1bd6742acff14f3fba53afc354782fbd5f6fc7b1421`  
		Last Modified: Mon, 23 May 2022 23:16:03 GMT  
		Size: 4.2 MB (4244908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251a42b41696b6a66317c2f99b1cd869dcdf07194f5f28e7edc10140fdf1acfd`  
		Last Modified: Mon, 23 May 2022 23:16:00 GMT  
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
$ docker pull nats@sha256:b368674b8858acdf4bdbb8bec04335cb6987fb1829159c212d781b689de74eea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4226009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2081876fa6098daea6a89b6894c8456c7b36939451c3d95d468ce493be85e1c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:40:25 GMT
COPY file:32e0c5d015acde93901500da0b0b479ba09cbb47d3918ad6d6b5523c686262ca in /nats-server 
# Mon, 23 May 2022 22:40:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:40:26 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:40:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:40:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:40:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7bdd5229d960e87b053609bd24bc82f46460a06899394029f599726df64da912`  
		Last Modified: Mon, 23 May 2022 22:41:46 GMT  
		Size: 4.2 MB (4225500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb661e40537a6e401894b3f7520bf397b6185ab575af1f5cf8bf40efcfd86bc`  
		Last Modified: Mon, 23 May 2022 22:41:45 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.2928; amd64

```console
$ docker pull nats@sha256:95b08fc423ab3d372702336dae5a8dbe2d1da429c18eeaf36f936fc0875ee7ac
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107772713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5d6c0f979e88d8401fee505a489498a7f206548060dfbf92e3adf4875a8ef8`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:42:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 23 May 2022 22:16:52 GMT
RUN cmd /S /C #(nop) COPY file:20c5da4e402adeb74e59df38a88afb7f0706725d1cf47a32deba2a95222bf05e in C:\nats-server.exe 
# Mon, 23 May 2022 22:16:53 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 23 May 2022 22:16:55 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2df39ac96d0b0efa546f2a05d81fb2a68ff8b0541fca6761bc2cedd28ff57f25`  
		Last Modified: Wed, 11 May 2022 14:43:01 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c75ab9a5e0f44e79c3adfc8b401bd352612bfa1c195e182dfedca24907fc2cb`  
		Last Modified: Mon, 23 May 2022 22:17:51 GMT  
		Size: 4.6 MB (4632778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7d580b9477c406ac03b52996e543c4d98651c583032c1cc8a15b97a42974d0`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.7 KB (1660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0c44352b5c88d59e36acd76446dfd0543670ed32caba214353a395b0e27590`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a07615e58e42c48f51d89c04072d98127ea7db787f97cdef0385b134fe681`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51272f4f628d52da760d5a41b2c254fe1082dbf88591529f520cc4d37a317a47`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:6052573e8a399a357cf0b7d84a694944aa016806d677a8026be807c56ce37354
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:2769de3270a9a86a1f799007cb1be2cbac229c07395206d13fbf845312481fc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7678717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0303f1d0cccc66a96da1353b9732b2b1b9dbd21206996b9af197b108e52d444b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 22:19:43 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:19:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 22:19:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 22:19:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 22:19:45 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:19:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 22:19:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68886d04807b30a327d175e97fe6fa560a6f4e68ea614397e87e7d456d6ace19`  
		Last Modified: Mon, 23 May 2022 22:20:18 GMT  
		Size: 4.9 MB (4863157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfc1bf8ce728acff89f87564fb40e67def44a450bd0e29f09309dad99e81ac6`  
		Last Modified: Mon, 23 May 2022 22:20:17 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c52785e040cd5cb0b784f0b7cf87f4ef40f0031383deb06acd3a5018bd0eee`  
		Last Modified: Mon, 23 May 2022 22:20:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:fcdca3dcbbb5b03284c64c0a9374301e1f7a901233a20a336949e932a510fd71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c863d799218e699e81cac4bbf925e850d19c0edf53ecabe58b02135444c6c01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 23:13:16 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 23:13:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 23:13:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 23:13:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 23:13:22 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 23:13:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 23:13:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b388d827d3aa697791f4a4d8097280f479f0faa6dc06e10f82c7653d34dcab`  
		Last Modified: Mon, 23 May 2022 23:15:27 GMT  
		Size: 4.5 MB (4518137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd801f49e3417e379c20c004c736e5b66baf62157ee6229ab1db746a0f665e46`  
		Last Modified: Mon, 23 May 2022 23:15:24 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877ff8ab778b23cf937adea367539b09513c39ed7e2af8f25a121793f7d0f68f`  
		Last Modified: Mon, 23 May 2022 23:15:24 GMT  
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
$ docker pull nats@sha256:adc4ca726f4e53b15e2a1d0d37aa7ff98c72bb2bd22fb72cac063d499b13bcba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7216231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f6313823af3524d1b2c8d4ce856935175e3ef55468eabfb142258efac8a00d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 22:40:07 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:40:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 22:40:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 22:40:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 22:40:12 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:40:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 22:40:14 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daa2cd1d5619c80b024c9f1d0980283c6ccd1a629a821540e044e4b1fdfcadf`  
		Last Modified: Mon, 23 May 2022 22:41:18 GMT  
		Size: 4.5 MB (4498780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ac0d288c25cbc55828b15cb671ae312a21835584b6c77e74cbd9513cb8813d`  
		Last Modified: Mon, 23 May 2022 22:41:17 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d9b1665dd8911a6f720bb3e6c144864b1907bd595f2141172a8a82bb0370ee`  
		Last Modified: Mon, 23 May 2022 22:41:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.15`

```console
$ docker pull nats@sha256:6052573e8a399a357cf0b7d84a694944aa016806d677a8026be807c56ce37354
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:2769de3270a9a86a1f799007cb1be2cbac229c07395206d13fbf845312481fc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7678717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0303f1d0cccc66a96da1353b9732b2b1b9dbd21206996b9af197b108e52d444b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 22:19:43 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:19:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 22:19:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 22:19:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 22:19:45 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:19:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 22:19:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68886d04807b30a327d175e97fe6fa560a6f4e68ea614397e87e7d456d6ace19`  
		Last Modified: Mon, 23 May 2022 22:20:18 GMT  
		Size: 4.9 MB (4863157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfc1bf8ce728acff89f87564fb40e67def44a450bd0e29f09309dad99e81ac6`  
		Last Modified: Mon, 23 May 2022 22:20:17 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c52785e040cd5cb0b784f0b7cf87f4ef40f0031383deb06acd3a5018bd0eee`  
		Last Modified: Mon, 23 May 2022 22:20:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:fcdca3dcbbb5b03284c64c0a9374301e1f7a901233a20a336949e932a510fd71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c863d799218e699e81cac4bbf925e850d19c0edf53ecabe58b02135444c6c01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 23:13:16 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 23:13:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 23:13:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 23:13:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 23:13:22 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 23:13:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 23:13:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b388d827d3aa697791f4a4d8097280f479f0faa6dc06e10f82c7653d34dcab`  
		Last Modified: Mon, 23 May 2022 23:15:27 GMT  
		Size: 4.5 MB (4518137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd801f49e3417e379c20c004c736e5b66baf62157ee6229ab1db746a0f665e46`  
		Last Modified: Mon, 23 May 2022 23:15:24 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877ff8ab778b23cf937adea367539b09513c39ed7e2af8f25a121793f7d0f68f`  
		Last Modified: Mon, 23 May 2022 23:15:24 GMT  
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
$ docker pull nats@sha256:adc4ca726f4e53b15e2a1d0d37aa7ff98c72bb2bd22fb72cac063d499b13bcba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7216231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f6313823af3524d1b2c8d4ce856935175e3ef55468eabfb142258efac8a00d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 22:40:07 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:40:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 22:40:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 22:40:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 22:40:12 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:40:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 22:40:14 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daa2cd1d5619c80b024c9f1d0980283c6ccd1a629a821540e044e4b1fdfcadf`  
		Last Modified: Mon, 23 May 2022 22:41:18 GMT  
		Size: 4.5 MB (4498780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ac0d288c25cbc55828b15cb671ae312a21835584b6c77e74cbd9513cb8813d`  
		Last Modified: Mon, 23 May 2022 22:41:17 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d9b1665dd8911a6f720bb3e6c144864b1907bd595f2141172a8a82bb0370ee`  
		Last Modified: Mon, 23 May 2022 22:41:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:f29655b29b519414dd885e07d7d4bdf22055d39406af47961dae06def8c7c600
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:c4c5aa8d8b2ce861febd7bd4dcd9a729204ba3f15f91fd96f45ab5a6e100e516
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4590377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ca6ed6836bb8a2f8705608091864ce3c25b8ca32693003e2a8df04e30dc0f9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:19:51 GMT
COPY file:8ff89c4fbf2c06b0c443f547e21c09f4d00bc37565795d87bfb43a04d4ff236e in /nats-server 
# Mon, 23 May 2022 22:19:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:19:51 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:19:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:19:52 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:19:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:49229864ce5450b6b5291aa946e418a9b56e6bbac1179c2a3ca592284b674f6c`  
		Last Modified: Mon, 23 May 2022 22:20:42 GMT  
		Size: 4.6 MB (4589871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f11a75312c73ef42e06951cc5acd4b2690648b1ab001bacda9622a11819993`  
		Last Modified: Mon, 23 May 2022 22:20:41 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:0a83bd61fe2f1ebbf052ab13bd453c3dfaec1db3e86896718024aff558174bf9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea45afb007d73aa5822eb21ef9e9d34b90edd8cbb44379c26a50b550889c3d3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 23:13:43 GMT
COPY file:4121ba71c4705779a334ba22404be19aaa6e3e8946ec6b5ce733466627f8c88e in /nats-server 
# Mon, 23 May 2022 23:13:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 23:13:44 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 23:13:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 23:13:45 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 23:13:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3429a8151ae5ab692b14a1bd6742acff14f3fba53afc354782fbd5f6fc7b1421`  
		Last Modified: Mon, 23 May 2022 23:16:03 GMT  
		Size: 4.2 MB (4244908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251a42b41696b6a66317c2f99b1cd869dcdf07194f5f28e7edc10140fdf1acfd`  
		Last Modified: Mon, 23 May 2022 23:16:00 GMT  
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
$ docker pull nats@sha256:b368674b8858acdf4bdbb8bec04335cb6987fb1829159c212d781b689de74eea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4226009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2081876fa6098daea6a89b6894c8456c7b36939451c3d95d468ce493be85e1c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:40:25 GMT
COPY file:32e0c5d015acde93901500da0b0b479ba09cbb47d3918ad6d6b5523c686262ca in /nats-server 
# Mon, 23 May 2022 22:40:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:40:26 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:40:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:40:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:40:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7bdd5229d960e87b053609bd24bc82f46460a06899394029f599726df64da912`  
		Last Modified: Mon, 23 May 2022 22:41:46 GMT  
		Size: 4.2 MB (4225500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb661e40537a6e401894b3f7520bf397b6185ab575af1f5cf8bf40efcfd86bc`  
		Last Modified: Mon, 23 May 2022 22:41:45 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:f338915431c6f74ef7061f9d4349709e849edca4a9f6492c84cce0132a9219f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.2928; amd64

```console
$ docker pull nats@sha256:95b08fc423ab3d372702336dae5a8dbe2d1da429c18eeaf36f936fc0875ee7ac
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107772713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5d6c0f979e88d8401fee505a489498a7f206548060dfbf92e3adf4875a8ef8`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:42:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 23 May 2022 22:16:52 GMT
RUN cmd /S /C #(nop) COPY file:20c5da4e402adeb74e59df38a88afb7f0706725d1cf47a32deba2a95222bf05e in C:\nats-server.exe 
# Mon, 23 May 2022 22:16:53 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 23 May 2022 22:16:55 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2df39ac96d0b0efa546f2a05d81fb2a68ff8b0541fca6761bc2cedd28ff57f25`  
		Last Modified: Wed, 11 May 2022 14:43:01 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c75ab9a5e0f44e79c3adfc8b401bd352612bfa1c195e182dfedca24907fc2cb`  
		Last Modified: Mon, 23 May 2022 22:17:51 GMT  
		Size: 4.6 MB (4632778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7d580b9477c406ac03b52996e543c4d98651c583032c1cc8a15b97a42974d0`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.7 KB (1660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0c44352b5c88d59e36acd76446dfd0543670ed32caba214353a395b0e27590`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a07615e58e42c48f51d89c04072d98127ea7db787f97cdef0385b134fe681`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51272f4f628d52da760d5a41b2c254fe1082dbf88591529f520cc4d37a317a47`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:f338915431c6f74ef7061f9d4349709e849edca4a9f6492c84cce0132a9219f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull nats@sha256:95b08fc423ab3d372702336dae5a8dbe2d1da429c18eeaf36f936fc0875ee7ac
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107772713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5d6c0f979e88d8401fee505a489498a7f206548060dfbf92e3adf4875a8ef8`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:42:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 23 May 2022 22:16:52 GMT
RUN cmd /S /C #(nop) COPY file:20c5da4e402adeb74e59df38a88afb7f0706725d1cf47a32deba2a95222bf05e in C:\nats-server.exe 
# Mon, 23 May 2022 22:16:53 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 23 May 2022 22:16:55 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2df39ac96d0b0efa546f2a05d81fb2a68ff8b0541fca6761bc2cedd28ff57f25`  
		Last Modified: Wed, 11 May 2022 14:43:01 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c75ab9a5e0f44e79c3adfc8b401bd352612bfa1c195e182dfedca24907fc2cb`  
		Last Modified: Mon, 23 May 2022 22:17:51 GMT  
		Size: 4.6 MB (4632778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7d580b9477c406ac03b52996e543c4d98651c583032c1cc8a15b97a42974d0`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.7 KB (1660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0c44352b5c88d59e36acd76446dfd0543670ed32caba214353a395b0e27590`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a07615e58e42c48f51d89c04072d98127ea7db787f97cdef0385b134fe681`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51272f4f628d52da760d5a41b2c254fe1082dbf88591529f520cc4d37a317a47`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:f29655b29b519414dd885e07d7d4bdf22055d39406af47961dae06def8c7c600
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:c4c5aa8d8b2ce861febd7bd4dcd9a729204ba3f15f91fd96f45ab5a6e100e516
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4590377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ca6ed6836bb8a2f8705608091864ce3c25b8ca32693003e2a8df04e30dc0f9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:19:51 GMT
COPY file:8ff89c4fbf2c06b0c443f547e21c09f4d00bc37565795d87bfb43a04d4ff236e in /nats-server 
# Mon, 23 May 2022 22:19:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:19:51 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:19:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:19:52 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:19:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:49229864ce5450b6b5291aa946e418a9b56e6bbac1179c2a3ca592284b674f6c`  
		Last Modified: Mon, 23 May 2022 22:20:42 GMT  
		Size: 4.6 MB (4589871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f11a75312c73ef42e06951cc5acd4b2690648b1ab001bacda9622a11819993`  
		Last Modified: Mon, 23 May 2022 22:20:41 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:0a83bd61fe2f1ebbf052ab13bd453c3dfaec1db3e86896718024aff558174bf9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea45afb007d73aa5822eb21ef9e9d34b90edd8cbb44379c26a50b550889c3d3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 23:13:43 GMT
COPY file:4121ba71c4705779a334ba22404be19aaa6e3e8946ec6b5ce733466627f8c88e in /nats-server 
# Mon, 23 May 2022 23:13:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 23:13:44 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 23:13:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 23:13:45 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 23:13:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3429a8151ae5ab692b14a1bd6742acff14f3fba53afc354782fbd5f6fc7b1421`  
		Last Modified: Mon, 23 May 2022 23:16:03 GMT  
		Size: 4.2 MB (4244908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251a42b41696b6a66317c2f99b1cd869dcdf07194f5f28e7edc10140fdf1acfd`  
		Last Modified: Mon, 23 May 2022 23:16:00 GMT  
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
$ docker pull nats@sha256:b368674b8858acdf4bdbb8bec04335cb6987fb1829159c212d781b689de74eea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4226009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2081876fa6098daea6a89b6894c8456c7b36939451c3d95d468ce493be85e1c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:40:25 GMT
COPY file:32e0c5d015acde93901500da0b0b479ba09cbb47d3918ad6d6b5523c686262ca in /nats-server 
# Mon, 23 May 2022 22:40:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:40:26 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:40:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:40:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:40:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7bdd5229d960e87b053609bd24bc82f46460a06899394029f599726df64da912`  
		Last Modified: Mon, 23 May 2022 22:41:46 GMT  
		Size: 4.2 MB (4225500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb661e40537a6e401894b3f7520bf397b6185ab575af1f5cf8bf40efcfd86bc`  
		Last Modified: Mon, 23 May 2022 22:41:45 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:eb36b93a9338c371fb136c3966ea0b1d41c268eb78dcc3f0cf4b4e4e6dc2f924
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.2928; amd64

```console
$ docker pull nats@sha256:463326eba88d62c6de77af4874f4dea9ef53d30a6606dc475205c5444dd14c81
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2509545826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5404ddeeb235704c9be25463973cf8749998a527098877629130155ee1a8de6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Wed, 11 May 2022 12:42:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 May 2022 14:39:53 GMT
ENV NATS_DOCKERIZED=1
# Mon, 23 May 2022 22:14:24 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:14:24 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.3/nats-server-v2.8.3-windows-amd64.zip
# Mon, 23 May 2022 22:14:25 GMT
ENV NATS_SERVER_SHASUM=8195903f1d389327041ed50dddd62715b6aa74cc3f8f94865a8ae7b5875b3851
# Mon, 23 May 2022 22:15:24 GMT
RUN Set-PSDebug -Trace 2
# Mon, 23 May 2022 22:16:37 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 23 May 2022 22:16:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Mon, 23 May 2022 22:16:39 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:16:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 23 May 2022 22:16:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b34adcbd607b6c175a7c7a819fecbbfd53899678f53f169f2b4504070ec6b0ab`  
		Last Modified: Wed, 11 May 2022 14:07:06 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0c1e63aec5d8d83ee6bf4eb10d12ff30fe2e0eee737a2ef9291ead11cfb5cc`  
		Last Modified: Wed, 11 May 2022 14:42:43 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57b75a2edf35183ae898a9d68d8f5198163c53e5451d8da3b6a181ea8fa457f`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44a0c943278e9a6934267b495e21157256a8e0e59112d219700f1569327f153`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df2fa385bec1c86f1db9e768adf0323d7ae63afc30b2b61659eb4da17fc1412`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a33a8f0bf09b30dd9167b4150806163869b35f9c43ea15769b422ef5eaa919f`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 497.4 KB (497358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf09bb112173ae8d9e2df16abe56deb21191a622f289250dbc71ecff4b8faf3`  
		Last Modified: Mon, 23 May 2022 22:17:31 GMT  
		Size: 5.0 MB (4980200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e5cc1fbe4cfbdbdeceba96cd585d66515fb4ef8e79b738fb3cff04474e6f6d`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.8 KB (1846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600c2585823168fbd8f9f26a1dda94da2579919da1485501b17c799a1968a86c`  
		Last Modified: Mon, 23 May 2022 22:17:26 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3960c981235519da3181138ec9e48ef481177d8129cccc3620327e71a7c29860`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c546fa758ac26156e07083b8d1919a68568872dace58969c4714577dddfc1a3`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:eb36b93a9338c371fb136c3966ea0b1d41c268eb78dcc3f0cf4b4e4e6dc2f924
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull nats@sha256:463326eba88d62c6de77af4874f4dea9ef53d30a6606dc475205c5444dd14c81
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2509545826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5404ddeeb235704c9be25463973cf8749998a527098877629130155ee1a8de6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Wed, 11 May 2022 12:42:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 May 2022 14:39:53 GMT
ENV NATS_DOCKERIZED=1
# Mon, 23 May 2022 22:14:24 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:14:24 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.3/nats-server-v2.8.3-windows-amd64.zip
# Mon, 23 May 2022 22:14:25 GMT
ENV NATS_SERVER_SHASUM=8195903f1d389327041ed50dddd62715b6aa74cc3f8f94865a8ae7b5875b3851
# Mon, 23 May 2022 22:15:24 GMT
RUN Set-PSDebug -Trace 2
# Mon, 23 May 2022 22:16:37 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 23 May 2022 22:16:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Mon, 23 May 2022 22:16:39 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:16:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 23 May 2022 22:16:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b34adcbd607b6c175a7c7a819fecbbfd53899678f53f169f2b4504070ec6b0ab`  
		Last Modified: Wed, 11 May 2022 14:07:06 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0c1e63aec5d8d83ee6bf4eb10d12ff30fe2e0eee737a2ef9291ead11cfb5cc`  
		Last Modified: Wed, 11 May 2022 14:42:43 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57b75a2edf35183ae898a9d68d8f5198163c53e5451d8da3b6a181ea8fa457f`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44a0c943278e9a6934267b495e21157256a8e0e59112d219700f1569327f153`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df2fa385bec1c86f1db9e768adf0323d7ae63afc30b2b61659eb4da17fc1412`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a33a8f0bf09b30dd9167b4150806163869b35f9c43ea15769b422ef5eaa919f`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 497.4 KB (497358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf09bb112173ae8d9e2df16abe56deb21191a622f289250dbc71ecff4b8faf3`  
		Last Modified: Mon, 23 May 2022 22:17:31 GMT  
		Size: 5.0 MB (4980200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e5cc1fbe4cfbdbdeceba96cd585d66515fb4ef8e79b738fb3cff04474e6f6d`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.8 KB (1846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600c2585823168fbd8f9f26a1dda94da2579919da1485501b17c799a1968a86c`  
		Last Modified: Mon, 23 May 2022 22:17:26 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3960c981235519da3181138ec9e48ef481177d8129cccc3620327e71a7c29860`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c546fa758ac26156e07083b8d1919a68568872dace58969c4714577dddfc1a3`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8`

```console
$ docker pull nats@sha256:faf79ebeddcf0d20856df247744cdf519e8051a2480cb12b9f53c4c2e0086b3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2928; amd64

### `nats:2.8` - linux; amd64

```console
$ docker pull nats@sha256:c4c5aa8d8b2ce861febd7bd4dcd9a729204ba3f15f91fd96f45ab5a6e100e516
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4590377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ca6ed6836bb8a2f8705608091864ce3c25b8ca32693003e2a8df04e30dc0f9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:19:51 GMT
COPY file:8ff89c4fbf2c06b0c443f547e21c09f4d00bc37565795d87bfb43a04d4ff236e in /nats-server 
# Mon, 23 May 2022 22:19:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:19:51 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:19:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:19:52 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:19:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:49229864ce5450b6b5291aa946e418a9b56e6bbac1179c2a3ca592284b674f6c`  
		Last Modified: Mon, 23 May 2022 22:20:42 GMT  
		Size: 4.6 MB (4589871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f11a75312c73ef42e06951cc5acd4b2690648b1ab001bacda9622a11819993`  
		Last Modified: Mon, 23 May 2022 22:20:41 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8` - linux; arm variant v6

```console
$ docker pull nats@sha256:0a83bd61fe2f1ebbf052ab13bd453c3dfaec1db3e86896718024aff558174bf9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea45afb007d73aa5822eb21ef9e9d34b90edd8cbb44379c26a50b550889c3d3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 23:13:43 GMT
COPY file:4121ba71c4705779a334ba22404be19aaa6e3e8946ec6b5ce733466627f8c88e in /nats-server 
# Mon, 23 May 2022 23:13:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 23:13:44 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 23:13:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 23:13:45 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 23:13:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3429a8151ae5ab692b14a1bd6742acff14f3fba53afc354782fbd5f6fc7b1421`  
		Last Modified: Mon, 23 May 2022 23:16:03 GMT  
		Size: 4.2 MB (4244908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251a42b41696b6a66317c2f99b1cd869dcdf07194f5f28e7edc10140fdf1acfd`  
		Last Modified: Mon, 23 May 2022 23:16:00 GMT  
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
$ docker pull nats@sha256:b368674b8858acdf4bdbb8bec04335cb6987fb1829159c212d781b689de74eea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4226009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2081876fa6098daea6a89b6894c8456c7b36939451c3d95d468ce493be85e1c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:40:25 GMT
COPY file:32e0c5d015acde93901500da0b0b479ba09cbb47d3918ad6d6b5523c686262ca in /nats-server 
# Mon, 23 May 2022 22:40:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:40:26 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:40:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:40:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:40:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7bdd5229d960e87b053609bd24bc82f46460a06899394029f599726df64da912`  
		Last Modified: Mon, 23 May 2022 22:41:46 GMT  
		Size: 4.2 MB (4225500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb661e40537a6e401894b3f7520bf397b6185ab575af1f5cf8bf40efcfd86bc`  
		Last Modified: Mon, 23 May 2022 22:41:45 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8` - windows version 10.0.17763.2928; amd64

```console
$ docker pull nats@sha256:95b08fc423ab3d372702336dae5a8dbe2d1da429c18eeaf36f936fc0875ee7ac
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107772713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5d6c0f979e88d8401fee505a489498a7f206548060dfbf92e3adf4875a8ef8`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:42:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 23 May 2022 22:16:52 GMT
RUN cmd /S /C #(nop) COPY file:20c5da4e402adeb74e59df38a88afb7f0706725d1cf47a32deba2a95222bf05e in C:\nats-server.exe 
# Mon, 23 May 2022 22:16:53 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 23 May 2022 22:16:55 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2df39ac96d0b0efa546f2a05d81fb2a68ff8b0541fca6761bc2cedd28ff57f25`  
		Last Modified: Wed, 11 May 2022 14:43:01 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c75ab9a5e0f44e79c3adfc8b401bd352612bfa1c195e182dfedca24907fc2cb`  
		Last Modified: Mon, 23 May 2022 22:17:51 GMT  
		Size: 4.6 MB (4632778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7d580b9477c406ac03b52996e543c4d98651c583032c1cc8a15b97a42974d0`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.7 KB (1660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0c44352b5c88d59e36acd76446dfd0543670ed32caba214353a395b0e27590`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a07615e58e42c48f51d89c04072d98127ea7db787f97cdef0385b134fe681`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51272f4f628d52da760d5a41b2c254fe1082dbf88591529f520cc4d37a317a47`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-alpine`

```console
$ docker pull nats@sha256:6052573e8a399a357cf0b7d84a694944aa016806d677a8026be807c56ce37354
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8-alpine` - linux; amd64

```console
$ docker pull nats@sha256:2769de3270a9a86a1f799007cb1be2cbac229c07395206d13fbf845312481fc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7678717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0303f1d0cccc66a96da1353b9732b2b1b9dbd21206996b9af197b108e52d444b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 22:19:43 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:19:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 22:19:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 22:19:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 22:19:45 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:19:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 22:19:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68886d04807b30a327d175e97fe6fa560a6f4e68ea614397e87e7d456d6ace19`  
		Last Modified: Mon, 23 May 2022 22:20:18 GMT  
		Size: 4.9 MB (4863157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfc1bf8ce728acff89f87564fb40e67def44a450bd0e29f09309dad99e81ac6`  
		Last Modified: Mon, 23 May 2022 22:20:17 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c52785e040cd5cb0b784f0b7cf87f4ef40f0031383deb06acd3a5018bd0eee`  
		Last Modified: Mon, 23 May 2022 22:20:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:fcdca3dcbbb5b03284c64c0a9374301e1f7a901233a20a336949e932a510fd71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c863d799218e699e81cac4bbf925e850d19c0edf53ecabe58b02135444c6c01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 23:13:16 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 23:13:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 23:13:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 23:13:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 23:13:22 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 23:13:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 23:13:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b388d827d3aa697791f4a4d8097280f479f0faa6dc06e10f82c7653d34dcab`  
		Last Modified: Mon, 23 May 2022 23:15:27 GMT  
		Size: 4.5 MB (4518137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd801f49e3417e379c20c004c736e5b66baf62157ee6229ab1db746a0f665e46`  
		Last Modified: Mon, 23 May 2022 23:15:24 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877ff8ab778b23cf937adea367539b09513c39ed7e2af8f25a121793f7d0f68f`  
		Last Modified: Mon, 23 May 2022 23:15:24 GMT  
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
$ docker pull nats@sha256:adc4ca726f4e53b15e2a1d0d37aa7ff98c72bb2bd22fb72cac063d499b13bcba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7216231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f6313823af3524d1b2c8d4ce856935175e3ef55468eabfb142258efac8a00d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 22:40:07 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:40:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 22:40:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 22:40:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 22:40:12 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:40:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 22:40:14 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daa2cd1d5619c80b024c9f1d0980283c6ccd1a629a821540e044e4b1fdfcadf`  
		Last Modified: Mon, 23 May 2022 22:41:18 GMT  
		Size: 4.5 MB (4498780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ac0d288c25cbc55828b15cb671ae312a21835584b6c77e74cbd9513cb8813d`  
		Last Modified: Mon, 23 May 2022 22:41:17 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d9b1665dd8911a6f720bb3e6c144864b1907bd595f2141172a8a82bb0370ee`  
		Last Modified: Mon, 23 May 2022 22:41:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-alpine3.15`

```console
$ docker pull nats@sha256:6052573e8a399a357cf0b7d84a694944aa016806d677a8026be807c56ce37354
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:2769de3270a9a86a1f799007cb1be2cbac229c07395206d13fbf845312481fc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7678717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0303f1d0cccc66a96da1353b9732b2b1b9dbd21206996b9af197b108e52d444b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 22:19:43 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:19:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 22:19:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 22:19:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 22:19:45 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:19:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 22:19:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68886d04807b30a327d175e97fe6fa560a6f4e68ea614397e87e7d456d6ace19`  
		Last Modified: Mon, 23 May 2022 22:20:18 GMT  
		Size: 4.9 MB (4863157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfc1bf8ce728acff89f87564fb40e67def44a450bd0e29f09309dad99e81ac6`  
		Last Modified: Mon, 23 May 2022 22:20:17 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c52785e040cd5cb0b784f0b7cf87f4ef40f0031383deb06acd3a5018bd0eee`  
		Last Modified: Mon, 23 May 2022 22:20:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:fcdca3dcbbb5b03284c64c0a9374301e1f7a901233a20a336949e932a510fd71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c863d799218e699e81cac4bbf925e850d19c0edf53ecabe58b02135444c6c01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 23:13:16 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 23:13:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 23:13:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 23:13:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 23:13:22 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 23:13:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 23:13:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b388d827d3aa697791f4a4d8097280f479f0faa6dc06e10f82c7653d34dcab`  
		Last Modified: Mon, 23 May 2022 23:15:27 GMT  
		Size: 4.5 MB (4518137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd801f49e3417e379c20c004c736e5b66baf62157ee6229ab1db746a0f665e46`  
		Last Modified: Mon, 23 May 2022 23:15:24 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877ff8ab778b23cf937adea367539b09513c39ed7e2af8f25a121793f7d0f68f`  
		Last Modified: Mon, 23 May 2022 23:15:24 GMT  
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
$ docker pull nats@sha256:adc4ca726f4e53b15e2a1d0d37aa7ff98c72bb2bd22fb72cac063d499b13bcba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7216231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f6313823af3524d1b2c8d4ce856935175e3ef55468eabfb142258efac8a00d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 22:40:07 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:40:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 22:40:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 22:40:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 22:40:12 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:40:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 22:40:14 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daa2cd1d5619c80b024c9f1d0980283c6ccd1a629a821540e044e4b1fdfcadf`  
		Last Modified: Mon, 23 May 2022 22:41:18 GMT  
		Size: 4.5 MB (4498780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ac0d288c25cbc55828b15cb671ae312a21835584b6c77e74cbd9513cb8813d`  
		Last Modified: Mon, 23 May 2022 22:41:17 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d9b1665dd8911a6f720bb3e6c144864b1907bd595f2141172a8a82bb0370ee`  
		Last Modified: Mon, 23 May 2022 22:41:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-linux`

```console
$ docker pull nats@sha256:f29655b29b519414dd885e07d7d4bdf22055d39406af47961dae06def8c7c600
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8-linux` - linux; amd64

```console
$ docker pull nats@sha256:c4c5aa8d8b2ce861febd7bd4dcd9a729204ba3f15f91fd96f45ab5a6e100e516
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4590377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ca6ed6836bb8a2f8705608091864ce3c25b8ca32693003e2a8df04e30dc0f9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:19:51 GMT
COPY file:8ff89c4fbf2c06b0c443f547e21c09f4d00bc37565795d87bfb43a04d4ff236e in /nats-server 
# Mon, 23 May 2022 22:19:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:19:51 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:19:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:19:52 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:19:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:49229864ce5450b6b5291aa946e418a9b56e6bbac1179c2a3ca592284b674f6c`  
		Last Modified: Mon, 23 May 2022 22:20:42 GMT  
		Size: 4.6 MB (4589871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f11a75312c73ef42e06951cc5acd4b2690648b1ab001bacda9622a11819993`  
		Last Modified: Mon, 23 May 2022 22:20:41 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:0a83bd61fe2f1ebbf052ab13bd453c3dfaec1db3e86896718024aff558174bf9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea45afb007d73aa5822eb21ef9e9d34b90edd8cbb44379c26a50b550889c3d3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 23:13:43 GMT
COPY file:4121ba71c4705779a334ba22404be19aaa6e3e8946ec6b5ce733466627f8c88e in /nats-server 
# Mon, 23 May 2022 23:13:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 23:13:44 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 23:13:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 23:13:45 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 23:13:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3429a8151ae5ab692b14a1bd6742acff14f3fba53afc354782fbd5f6fc7b1421`  
		Last Modified: Mon, 23 May 2022 23:16:03 GMT  
		Size: 4.2 MB (4244908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251a42b41696b6a66317c2f99b1cd869dcdf07194f5f28e7edc10140fdf1acfd`  
		Last Modified: Mon, 23 May 2022 23:16:00 GMT  
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
$ docker pull nats@sha256:b368674b8858acdf4bdbb8bec04335cb6987fb1829159c212d781b689de74eea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4226009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2081876fa6098daea6a89b6894c8456c7b36939451c3d95d468ce493be85e1c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:40:25 GMT
COPY file:32e0c5d015acde93901500da0b0b479ba09cbb47d3918ad6d6b5523c686262ca in /nats-server 
# Mon, 23 May 2022 22:40:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:40:26 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:40:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:40:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:40:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7bdd5229d960e87b053609bd24bc82f46460a06899394029f599726df64da912`  
		Last Modified: Mon, 23 May 2022 22:41:46 GMT  
		Size: 4.2 MB (4225500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb661e40537a6e401894b3f7520bf397b6185ab575af1f5cf8bf40efcfd86bc`  
		Last Modified: Mon, 23 May 2022 22:41:45 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-nanoserver`

```console
$ docker pull nats@sha256:f338915431c6f74ef7061f9d4349709e849edca4a9f6492c84cce0132a9219f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `nats:2.8-nanoserver` - windows version 10.0.17763.2928; amd64

```console
$ docker pull nats@sha256:95b08fc423ab3d372702336dae5a8dbe2d1da429c18eeaf36f936fc0875ee7ac
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107772713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5d6c0f979e88d8401fee505a489498a7f206548060dfbf92e3adf4875a8ef8`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:42:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 23 May 2022 22:16:52 GMT
RUN cmd /S /C #(nop) COPY file:20c5da4e402adeb74e59df38a88afb7f0706725d1cf47a32deba2a95222bf05e in C:\nats-server.exe 
# Mon, 23 May 2022 22:16:53 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 23 May 2022 22:16:55 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2df39ac96d0b0efa546f2a05d81fb2a68ff8b0541fca6761bc2cedd28ff57f25`  
		Last Modified: Wed, 11 May 2022 14:43:01 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c75ab9a5e0f44e79c3adfc8b401bd352612bfa1c195e182dfedca24907fc2cb`  
		Last Modified: Mon, 23 May 2022 22:17:51 GMT  
		Size: 4.6 MB (4632778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7d580b9477c406ac03b52996e543c4d98651c583032c1cc8a15b97a42974d0`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.7 KB (1660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0c44352b5c88d59e36acd76446dfd0543670ed32caba214353a395b0e27590`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a07615e58e42c48f51d89c04072d98127ea7db787f97cdef0385b134fe681`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51272f4f628d52da760d5a41b2c254fe1082dbf88591529f520cc4d37a317a47`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-nanoserver-1809`

```console
$ docker pull nats@sha256:f338915431c6f74ef7061f9d4349709e849edca4a9f6492c84cce0132a9219f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `nats:2.8-nanoserver-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull nats@sha256:95b08fc423ab3d372702336dae5a8dbe2d1da429c18eeaf36f936fc0875ee7ac
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107772713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5d6c0f979e88d8401fee505a489498a7f206548060dfbf92e3adf4875a8ef8`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:42:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 23 May 2022 22:16:52 GMT
RUN cmd /S /C #(nop) COPY file:20c5da4e402adeb74e59df38a88afb7f0706725d1cf47a32deba2a95222bf05e in C:\nats-server.exe 
# Mon, 23 May 2022 22:16:53 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 23 May 2022 22:16:55 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2df39ac96d0b0efa546f2a05d81fb2a68ff8b0541fca6761bc2cedd28ff57f25`  
		Last Modified: Wed, 11 May 2022 14:43:01 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c75ab9a5e0f44e79c3adfc8b401bd352612bfa1c195e182dfedca24907fc2cb`  
		Last Modified: Mon, 23 May 2022 22:17:51 GMT  
		Size: 4.6 MB (4632778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7d580b9477c406ac03b52996e543c4d98651c583032c1cc8a15b97a42974d0`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.7 KB (1660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0c44352b5c88d59e36acd76446dfd0543670ed32caba214353a395b0e27590`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a07615e58e42c48f51d89c04072d98127ea7db787f97cdef0385b134fe681`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51272f4f628d52da760d5a41b2c254fe1082dbf88591529f520cc4d37a317a47`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-scratch`

```console
$ docker pull nats@sha256:f29655b29b519414dd885e07d7d4bdf22055d39406af47961dae06def8c7c600
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.8-scratch` - linux; amd64

```console
$ docker pull nats@sha256:c4c5aa8d8b2ce861febd7bd4dcd9a729204ba3f15f91fd96f45ab5a6e100e516
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4590377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ca6ed6836bb8a2f8705608091864ce3c25b8ca32693003e2a8df04e30dc0f9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:19:51 GMT
COPY file:8ff89c4fbf2c06b0c443f547e21c09f4d00bc37565795d87bfb43a04d4ff236e in /nats-server 
# Mon, 23 May 2022 22:19:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:19:51 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:19:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:19:52 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:19:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:49229864ce5450b6b5291aa946e418a9b56e6bbac1179c2a3ca592284b674f6c`  
		Last Modified: Mon, 23 May 2022 22:20:42 GMT  
		Size: 4.6 MB (4589871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f11a75312c73ef42e06951cc5acd4b2690648b1ab001bacda9622a11819993`  
		Last Modified: Mon, 23 May 2022 22:20:41 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:0a83bd61fe2f1ebbf052ab13bd453c3dfaec1db3e86896718024aff558174bf9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea45afb007d73aa5822eb21ef9e9d34b90edd8cbb44379c26a50b550889c3d3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 23:13:43 GMT
COPY file:4121ba71c4705779a334ba22404be19aaa6e3e8946ec6b5ce733466627f8c88e in /nats-server 
# Mon, 23 May 2022 23:13:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 23:13:44 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 23:13:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 23:13:45 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 23:13:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3429a8151ae5ab692b14a1bd6742acff14f3fba53afc354782fbd5f6fc7b1421`  
		Last Modified: Mon, 23 May 2022 23:16:03 GMT  
		Size: 4.2 MB (4244908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251a42b41696b6a66317c2f99b1cd869dcdf07194f5f28e7edc10140fdf1acfd`  
		Last Modified: Mon, 23 May 2022 23:16:00 GMT  
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
$ docker pull nats@sha256:b368674b8858acdf4bdbb8bec04335cb6987fb1829159c212d781b689de74eea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4226009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2081876fa6098daea6a89b6894c8456c7b36939451c3d95d468ce493be85e1c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:40:25 GMT
COPY file:32e0c5d015acde93901500da0b0b479ba09cbb47d3918ad6d6b5523c686262ca in /nats-server 
# Mon, 23 May 2022 22:40:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:40:26 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:40:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:40:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:40:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7bdd5229d960e87b053609bd24bc82f46460a06899394029f599726df64da912`  
		Last Modified: Mon, 23 May 2022 22:41:46 GMT  
		Size: 4.2 MB (4225500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb661e40537a6e401894b3f7520bf397b6185ab575af1f5cf8bf40efcfd86bc`  
		Last Modified: Mon, 23 May 2022 22:41:45 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-windowsservercore`

```console
$ docker pull nats@sha256:eb36b93a9338c371fb136c3966ea0b1d41c268eb78dcc3f0cf4b4e4e6dc2f924
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `nats:2.8-windowsservercore` - windows version 10.0.17763.2928; amd64

```console
$ docker pull nats@sha256:463326eba88d62c6de77af4874f4dea9ef53d30a6606dc475205c5444dd14c81
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2509545826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5404ddeeb235704c9be25463973cf8749998a527098877629130155ee1a8de6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Wed, 11 May 2022 12:42:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 May 2022 14:39:53 GMT
ENV NATS_DOCKERIZED=1
# Mon, 23 May 2022 22:14:24 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:14:24 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.3/nats-server-v2.8.3-windows-amd64.zip
# Mon, 23 May 2022 22:14:25 GMT
ENV NATS_SERVER_SHASUM=8195903f1d389327041ed50dddd62715b6aa74cc3f8f94865a8ae7b5875b3851
# Mon, 23 May 2022 22:15:24 GMT
RUN Set-PSDebug -Trace 2
# Mon, 23 May 2022 22:16:37 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 23 May 2022 22:16:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Mon, 23 May 2022 22:16:39 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:16:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 23 May 2022 22:16:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b34adcbd607b6c175a7c7a819fecbbfd53899678f53f169f2b4504070ec6b0ab`  
		Last Modified: Wed, 11 May 2022 14:07:06 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0c1e63aec5d8d83ee6bf4eb10d12ff30fe2e0eee737a2ef9291ead11cfb5cc`  
		Last Modified: Wed, 11 May 2022 14:42:43 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57b75a2edf35183ae898a9d68d8f5198163c53e5451d8da3b6a181ea8fa457f`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44a0c943278e9a6934267b495e21157256a8e0e59112d219700f1569327f153`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df2fa385bec1c86f1db9e768adf0323d7ae63afc30b2b61659eb4da17fc1412`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a33a8f0bf09b30dd9167b4150806163869b35f9c43ea15769b422ef5eaa919f`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 497.4 KB (497358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf09bb112173ae8d9e2df16abe56deb21191a622f289250dbc71ecff4b8faf3`  
		Last Modified: Mon, 23 May 2022 22:17:31 GMT  
		Size: 5.0 MB (4980200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e5cc1fbe4cfbdbdeceba96cd585d66515fb4ef8e79b738fb3cff04474e6f6d`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.8 KB (1846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600c2585823168fbd8f9f26a1dda94da2579919da1485501b17c799a1968a86c`  
		Last Modified: Mon, 23 May 2022 22:17:26 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3960c981235519da3181138ec9e48ef481177d8129cccc3620327e71a7c29860`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c546fa758ac26156e07083b8d1919a68568872dace58969c4714577dddfc1a3`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8-windowsservercore-1809`

```console
$ docker pull nats@sha256:eb36b93a9338c371fb136c3966ea0b1d41c268eb78dcc3f0cf4b4e4e6dc2f924
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `nats:2.8-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull nats@sha256:463326eba88d62c6de77af4874f4dea9ef53d30a6606dc475205c5444dd14c81
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2509545826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5404ddeeb235704c9be25463973cf8749998a527098877629130155ee1a8de6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Wed, 11 May 2022 12:42:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 May 2022 14:39:53 GMT
ENV NATS_DOCKERIZED=1
# Mon, 23 May 2022 22:14:24 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:14:24 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.3/nats-server-v2.8.3-windows-amd64.zip
# Mon, 23 May 2022 22:14:25 GMT
ENV NATS_SERVER_SHASUM=8195903f1d389327041ed50dddd62715b6aa74cc3f8f94865a8ae7b5875b3851
# Mon, 23 May 2022 22:15:24 GMT
RUN Set-PSDebug -Trace 2
# Mon, 23 May 2022 22:16:37 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 23 May 2022 22:16:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Mon, 23 May 2022 22:16:39 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:16:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 23 May 2022 22:16:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b34adcbd607b6c175a7c7a819fecbbfd53899678f53f169f2b4504070ec6b0ab`  
		Last Modified: Wed, 11 May 2022 14:07:06 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0c1e63aec5d8d83ee6bf4eb10d12ff30fe2e0eee737a2ef9291ead11cfb5cc`  
		Last Modified: Wed, 11 May 2022 14:42:43 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57b75a2edf35183ae898a9d68d8f5198163c53e5451d8da3b6a181ea8fa457f`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44a0c943278e9a6934267b495e21157256a8e0e59112d219700f1569327f153`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df2fa385bec1c86f1db9e768adf0323d7ae63afc30b2b61659eb4da17fc1412`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a33a8f0bf09b30dd9167b4150806163869b35f9c43ea15769b422ef5eaa919f`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 497.4 KB (497358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf09bb112173ae8d9e2df16abe56deb21191a622f289250dbc71ecff4b8faf3`  
		Last Modified: Mon, 23 May 2022 22:17:31 GMT  
		Size: 5.0 MB (4980200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e5cc1fbe4cfbdbdeceba96cd585d66515fb4ef8e79b738fb3cff04474e6f6d`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.8 KB (1846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600c2585823168fbd8f9f26a1dda94da2579919da1485501b17c799a1968a86c`  
		Last Modified: Mon, 23 May 2022 22:17:26 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3960c981235519da3181138ec9e48ef481177d8129cccc3620327e71a7c29860`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c546fa758ac26156e07083b8d1919a68568872dace58969c4714577dddfc1a3`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.3`

```console
$ docker pull nats@sha256:f01c3f668cf292a41ca5c8313ca1636536628ac71cbdc10bff4f951441c6bb63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2928; amd64

### `nats:2.8.3` - linux; amd64

```console
$ docker pull nats@sha256:c4c5aa8d8b2ce861febd7bd4dcd9a729204ba3f15f91fd96f45ab5a6e100e516
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4590377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ca6ed6836bb8a2f8705608091864ce3c25b8ca32693003e2a8df04e30dc0f9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:19:51 GMT
COPY file:8ff89c4fbf2c06b0c443f547e21c09f4d00bc37565795d87bfb43a04d4ff236e in /nats-server 
# Mon, 23 May 2022 22:19:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:19:51 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:19:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:19:52 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:19:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:49229864ce5450b6b5291aa946e418a9b56e6bbac1179c2a3ca592284b674f6c`  
		Last Modified: Mon, 23 May 2022 22:20:42 GMT  
		Size: 4.6 MB (4589871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f11a75312c73ef42e06951cc5acd4b2690648b1ab001bacda9622a11819993`  
		Last Modified: Mon, 23 May 2022 22:20:41 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.3` - linux; arm variant v6

```console
$ docker pull nats@sha256:0a83bd61fe2f1ebbf052ab13bd453c3dfaec1db3e86896718024aff558174bf9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea45afb007d73aa5822eb21ef9e9d34b90edd8cbb44379c26a50b550889c3d3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 23:13:43 GMT
COPY file:4121ba71c4705779a334ba22404be19aaa6e3e8946ec6b5ce733466627f8c88e in /nats-server 
# Mon, 23 May 2022 23:13:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 23:13:44 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 23:13:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 23:13:45 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 23:13:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3429a8151ae5ab692b14a1bd6742acff14f3fba53afc354782fbd5f6fc7b1421`  
		Last Modified: Mon, 23 May 2022 23:16:03 GMT  
		Size: 4.2 MB (4244908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251a42b41696b6a66317c2f99b1cd869dcdf07194f5f28e7edc10140fdf1acfd`  
		Last Modified: Mon, 23 May 2022 23:16:00 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.3` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b368674b8858acdf4bdbb8bec04335cb6987fb1829159c212d781b689de74eea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4226009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2081876fa6098daea6a89b6894c8456c7b36939451c3d95d468ce493be85e1c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:40:25 GMT
COPY file:32e0c5d015acde93901500da0b0b479ba09cbb47d3918ad6d6b5523c686262ca in /nats-server 
# Mon, 23 May 2022 22:40:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:40:26 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:40:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:40:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:40:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7bdd5229d960e87b053609bd24bc82f46460a06899394029f599726df64da912`  
		Last Modified: Mon, 23 May 2022 22:41:46 GMT  
		Size: 4.2 MB (4225500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb661e40537a6e401894b3f7520bf397b6185ab575af1f5cf8bf40efcfd86bc`  
		Last Modified: Mon, 23 May 2022 22:41:45 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.3` - windows version 10.0.17763.2928; amd64

```console
$ docker pull nats@sha256:95b08fc423ab3d372702336dae5a8dbe2d1da429c18eeaf36f936fc0875ee7ac
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107772713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5d6c0f979e88d8401fee505a489498a7f206548060dfbf92e3adf4875a8ef8`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:42:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 23 May 2022 22:16:52 GMT
RUN cmd /S /C #(nop) COPY file:20c5da4e402adeb74e59df38a88afb7f0706725d1cf47a32deba2a95222bf05e in C:\nats-server.exe 
# Mon, 23 May 2022 22:16:53 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 23 May 2022 22:16:55 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2df39ac96d0b0efa546f2a05d81fb2a68ff8b0541fca6761bc2cedd28ff57f25`  
		Last Modified: Wed, 11 May 2022 14:43:01 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c75ab9a5e0f44e79c3adfc8b401bd352612bfa1c195e182dfedca24907fc2cb`  
		Last Modified: Mon, 23 May 2022 22:17:51 GMT  
		Size: 4.6 MB (4632778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7d580b9477c406ac03b52996e543c4d98651c583032c1cc8a15b97a42974d0`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.7 KB (1660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0c44352b5c88d59e36acd76446dfd0543670ed32caba214353a395b0e27590`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a07615e58e42c48f51d89c04072d98127ea7db787f97cdef0385b134fe681`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51272f4f628d52da760d5a41b2c254fe1082dbf88591529f520cc4d37a317a47`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.3-alpine`

```console
$ docker pull nats@sha256:8967e79c1b5a8ec8794fcc567675aaa57d4330795230cccfbd9ffeb7a18e7a42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.8.3-alpine` - linux; amd64

```console
$ docker pull nats@sha256:2769de3270a9a86a1f799007cb1be2cbac229c07395206d13fbf845312481fc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7678717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0303f1d0cccc66a96da1353b9732b2b1b9dbd21206996b9af197b108e52d444b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 22:19:43 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:19:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 22:19:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 22:19:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 22:19:45 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:19:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 22:19:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68886d04807b30a327d175e97fe6fa560a6f4e68ea614397e87e7d456d6ace19`  
		Last Modified: Mon, 23 May 2022 22:20:18 GMT  
		Size: 4.9 MB (4863157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfc1bf8ce728acff89f87564fb40e67def44a450bd0e29f09309dad99e81ac6`  
		Last Modified: Mon, 23 May 2022 22:20:17 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c52785e040cd5cb0b784f0b7cf87f4ef40f0031383deb06acd3a5018bd0eee`  
		Last Modified: Mon, 23 May 2022 22:20:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.3-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:fcdca3dcbbb5b03284c64c0a9374301e1f7a901233a20a336949e932a510fd71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c863d799218e699e81cac4bbf925e850d19c0edf53ecabe58b02135444c6c01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 23:13:16 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 23:13:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 23:13:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 23:13:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 23:13:22 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 23:13:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 23:13:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b388d827d3aa697791f4a4d8097280f479f0faa6dc06e10f82c7653d34dcab`  
		Last Modified: Mon, 23 May 2022 23:15:27 GMT  
		Size: 4.5 MB (4518137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd801f49e3417e379c20c004c736e5b66baf62157ee6229ab1db746a0f665e46`  
		Last Modified: Mon, 23 May 2022 23:15:24 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877ff8ab778b23cf937adea367539b09513c39ed7e2af8f25a121793f7d0f68f`  
		Last Modified: Mon, 23 May 2022 23:15:24 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.3-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:adc4ca726f4e53b15e2a1d0d37aa7ff98c72bb2bd22fb72cac063d499b13bcba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7216231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f6313823af3524d1b2c8d4ce856935175e3ef55468eabfb142258efac8a00d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 22:40:07 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:40:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 22:40:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 22:40:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 22:40:12 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:40:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 22:40:14 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daa2cd1d5619c80b024c9f1d0980283c6ccd1a629a821540e044e4b1fdfcadf`  
		Last Modified: Mon, 23 May 2022 22:41:18 GMT  
		Size: 4.5 MB (4498780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ac0d288c25cbc55828b15cb671ae312a21835584b6c77e74cbd9513cb8813d`  
		Last Modified: Mon, 23 May 2022 22:41:17 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d9b1665dd8911a6f720bb3e6c144864b1907bd595f2141172a8a82bb0370ee`  
		Last Modified: Mon, 23 May 2022 22:41:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.3-alpine3.15`

```console
$ docker pull nats@sha256:8967e79c1b5a8ec8794fcc567675aaa57d4330795230cccfbd9ffeb7a18e7a42
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.8.3-alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:2769de3270a9a86a1f799007cb1be2cbac229c07395206d13fbf845312481fc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7678717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0303f1d0cccc66a96da1353b9732b2b1b9dbd21206996b9af197b108e52d444b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 22:19:43 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:19:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 22:19:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 22:19:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 22:19:45 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:19:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 22:19:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68886d04807b30a327d175e97fe6fa560a6f4e68ea614397e87e7d456d6ace19`  
		Last Modified: Mon, 23 May 2022 22:20:18 GMT  
		Size: 4.9 MB (4863157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfc1bf8ce728acff89f87564fb40e67def44a450bd0e29f09309dad99e81ac6`  
		Last Modified: Mon, 23 May 2022 22:20:17 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c52785e040cd5cb0b784f0b7cf87f4ef40f0031383deb06acd3a5018bd0eee`  
		Last Modified: Mon, 23 May 2022 22:20:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.3-alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:fcdca3dcbbb5b03284c64c0a9374301e1f7a901233a20a336949e932a510fd71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c863d799218e699e81cac4bbf925e850d19c0edf53ecabe58b02135444c6c01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 23:13:16 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 23:13:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 23:13:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 23:13:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 23:13:22 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 23:13:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 23:13:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b388d827d3aa697791f4a4d8097280f479f0faa6dc06e10f82c7653d34dcab`  
		Last Modified: Mon, 23 May 2022 23:15:27 GMT  
		Size: 4.5 MB (4518137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd801f49e3417e379c20c004c736e5b66baf62157ee6229ab1db746a0f665e46`  
		Last Modified: Mon, 23 May 2022 23:15:24 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877ff8ab778b23cf937adea367539b09513c39ed7e2af8f25a121793f7d0f68f`  
		Last Modified: Mon, 23 May 2022 23:15:24 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.3-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:adc4ca726f4e53b15e2a1d0d37aa7ff98c72bb2bd22fb72cac063d499b13bcba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7216231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f6313823af3524d1b2c8d4ce856935175e3ef55468eabfb142258efac8a00d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 22:40:07 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:40:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 22:40:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 22:40:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 22:40:12 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:40:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 22:40:14 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daa2cd1d5619c80b024c9f1d0980283c6ccd1a629a821540e044e4b1fdfcadf`  
		Last Modified: Mon, 23 May 2022 22:41:18 GMT  
		Size: 4.5 MB (4498780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ac0d288c25cbc55828b15cb671ae312a21835584b6c77e74cbd9513cb8813d`  
		Last Modified: Mon, 23 May 2022 22:41:17 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d9b1665dd8911a6f720bb3e6c144864b1907bd595f2141172a8a82bb0370ee`  
		Last Modified: Mon, 23 May 2022 22:41:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.3-linux`

```console
$ docker pull nats@sha256:febca974b215473d08d637e7325745d2adf853ae3648cd5530998448a0d473db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.8.3-linux` - linux; amd64

```console
$ docker pull nats@sha256:c4c5aa8d8b2ce861febd7bd4dcd9a729204ba3f15f91fd96f45ab5a6e100e516
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4590377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ca6ed6836bb8a2f8705608091864ce3c25b8ca32693003e2a8df04e30dc0f9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:19:51 GMT
COPY file:8ff89c4fbf2c06b0c443f547e21c09f4d00bc37565795d87bfb43a04d4ff236e in /nats-server 
# Mon, 23 May 2022 22:19:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:19:51 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:19:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:19:52 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:19:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:49229864ce5450b6b5291aa946e418a9b56e6bbac1179c2a3ca592284b674f6c`  
		Last Modified: Mon, 23 May 2022 22:20:42 GMT  
		Size: 4.6 MB (4589871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f11a75312c73ef42e06951cc5acd4b2690648b1ab001bacda9622a11819993`  
		Last Modified: Mon, 23 May 2022 22:20:41 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.3-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:0a83bd61fe2f1ebbf052ab13bd453c3dfaec1db3e86896718024aff558174bf9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea45afb007d73aa5822eb21ef9e9d34b90edd8cbb44379c26a50b550889c3d3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 23:13:43 GMT
COPY file:4121ba71c4705779a334ba22404be19aaa6e3e8946ec6b5ce733466627f8c88e in /nats-server 
# Mon, 23 May 2022 23:13:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 23:13:44 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 23:13:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 23:13:45 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 23:13:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3429a8151ae5ab692b14a1bd6742acff14f3fba53afc354782fbd5f6fc7b1421`  
		Last Modified: Mon, 23 May 2022 23:16:03 GMT  
		Size: 4.2 MB (4244908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251a42b41696b6a66317c2f99b1cd869dcdf07194f5f28e7edc10140fdf1acfd`  
		Last Modified: Mon, 23 May 2022 23:16:00 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.3-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b368674b8858acdf4bdbb8bec04335cb6987fb1829159c212d781b689de74eea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4226009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2081876fa6098daea6a89b6894c8456c7b36939451c3d95d468ce493be85e1c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:40:25 GMT
COPY file:32e0c5d015acde93901500da0b0b479ba09cbb47d3918ad6d6b5523c686262ca in /nats-server 
# Mon, 23 May 2022 22:40:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:40:26 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:40:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:40:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:40:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7bdd5229d960e87b053609bd24bc82f46460a06899394029f599726df64da912`  
		Last Modified: Mon, 23 May 2022 22:41:46 GMT  
		Size: 4.2 MB (4225500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb661e40537a6e401894b3f7520bf397b6185ab575af1f5cf8bf40efcfd86bc`  
		Last Modified: Mon, 23 May 2022 22:41:45 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.3-nanoserver`

```console
$ docker pull nats@sha256:f338915431c6f74ef7061f9d4349709e849edca4a9f6492c84cce0132a9219f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `nats:2.8.3-nanoserver` - windows version 10.0.17763.2928; amd64

```console
$ docker pull nats@sha256:95b08fc423ab3d372702336dae5a8dbe2d1da429c18eeaf36f936fc0875ee7ac
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107772713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5d6c0f979e88d8401fee505a489498a7f206548060dfbf92e3adf4875a8ef8`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:42:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 23 May 2022 22:16:52 GMT
RUN cmd /S /C #(nop) COPY file:20c5da4e402adeb74e59df38a88afb7f0706725d1cf47a32deba2a95222bf05e in C:\nats-server.exe 
# Mon, 23 May 2022 22:16:53 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 23 May 2022 22:16:55 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2df39ac96d0b0efa546f2a05d81fb2a68ff8b0541fca6761bc2cedd28ff57f25`  
		Last Modified: Wed, 11 May 2022 14:43:01 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c75ab9a5e0f44e79c3adfc8b401bd352612bfa1c195e182dfedca24907fc2cb`  
		Last Modified: Mon, 23 May 2022 22:17:51 GMT  
		Size: 4.6 MB (4632778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7d580b9477c406ac03b52996e543c4d98651c583032c1cc8a15b97a42974d0`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.7 KB (1660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0c44352b5c88d59e36acd76446dfd0543670ed32caba214353a395b0e27590`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a07615e58e42c48f51d89c04072d98127ea7db787f97cdef0385b134fe681`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51272f4f628d52da760d5a41b2c254fe1082dbf88591529f520cc4d37a317a47`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.3-nanoserver-1809`

```console
$ docker pull nats@sha256:f338915431c6f74ef7061f9d4349709e849edca4a9f6492c84cce0132a9219f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `nats:2.8.3-nanoserver-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull nats@sha256:95b08fc423ab3d372702336dae5a8dbe2d1da429c18eeaf36f936fc0875ee7ac
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107772713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5d6c0f979e88d8401fee505a489498a7f206548060dfbf92e3adf4875a8ef8`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:42:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 23 May 2022 22:16:52 GMT
RUN cmd /S /C #(nop) COPY file:20c5da4e402adeb74e59df38a88afb7f0706725d1cf47a32deba2a95222bf05e in C:\nats-server.exe 
# Mon, 23 May 2022 22:16:53 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 23 May 2022 22:16:55 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2df39ac96d0b0efa546f2a05d81fb2a68ff8b0541fca6761bc2cedd28ff57f25`  
		Last Modified: Wed, 11 May 2022 14:43:01 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c75ab9a5e0f44e79c3adfc8b401bd352612bfa1c195e182dfedca24907fc2cb`  
		Last Modified: Mon, 23 May 2022 22:17:51 GMT  
		Size: 4.6 MB (4632778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7d580b9477c406ac03b52996e543c4d98651c583032c1cc8a15b97a42974d0`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.7 KB (1660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0c44352b5c88d59e36acd76446dfd0543670ed32caba214353a395b0e27590`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a07615e58e42c48f51d89c04072d98127ea7db787f97cdef0385b134fe681`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51272f4f628d52da760d5a41b2c254fe1082dbf88591529f520cc4d37a317a47`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.3-scratch`

```console
$ docker pull nats@sha256:febca974b215473d08d637e7325745d2adf853ae3648cd5530998448a0d473db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8

### `nats:2.8.3-scratch` - linux; amd64

```console
$ docker pull nats@sha256:c4c5aa8d8b2ce861febd7bd4dcd9a729204ba3f15f91fd96f45ab5a6e100e516
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4590377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ca6ed6836bb8a2f8705608091864ce3c25b8ca32693003e2a8df04e30dc0f9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:19:51 GMT
COPY file:8ff89c4fbf2c06b0c443f547e21c09f4d00bc37565795d87bfb43a04d4ff236e in /nats-server 
# Mon, 23 May 2022 22:19:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:19:51 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:19:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:19:52 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:19:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:49229864ce5450b6b5291aa946e418a9b56e6bbac1179c2a3ca592284b674f6c`  
		Last Modified: Mon, 23 May 2022 22:20:42 GMT  
		Size: 4.6 MB (4589871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f11a75312c73ef42e06951cc5acd4b2690648b1ab001bacda9622a11819993`  
		Last Modified: Mon, 23 May 2022 22:20:41 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.3-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:0a83bd61fe2f1ebbf052ab13bd453c3dfaec1db3e86896718024aff558174bf9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea45afb007d73aa5822eb21ef9e9d34b90edd8cbb44379c26a50b550889c3d3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 23:13:43 GMT
COPY file:4121ba71c4705779a334ba22404be19aaa6e3e8946ec6b5ce733466627f8c88e in /nats-server 
# Mon, 23 May 2022 23:13:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 23:13:44 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 23:13:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 23:13:45 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 23:13:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3429a8151ae5ab692b14a1bd6742acff14f3fba53afc354782fbd5f6fc7b1421`  
		Last Modified: Mon, 23 May 2022 23:16:03 GMT  
		Size: 4.2 MB (4244908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251a42b41696b6a66317c2f99b1cd869dcdf07194f5f28e7edc10140fdf1acfd`  
		Last Modified: Mon, 23 May 2022 23:16:00 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.8.3-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b368674b8858acdf4bdbb8bec04335cb6987fb1829159c212d781b689de74eea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4226009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2081876fa6098daea6a89b6894c8456c7b36939451c3d95d468ce493be85e1c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:40:25 GMT
COPY file:32e0c5d015acde93901500da0b0b479ba09cbb47d3918ad6d6b5523c686262ca in /nats-server 
# Mon, 23 May 2022 22:40:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:40:26 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:40:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:40:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:40:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7bdd5229d960e87b053609bd24bc82f46460a06899394029f599726df64da912`  
		Last Modified: Mon, 23 May 2022 22:41:46 GMT  
		Size: 4.2 MB (4225500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb661e40537a6e401894b3f7520bf397b6185ab575af1f5cf8bf40efcfd86bc`  
		Last Modified: Mon, 23 May 2022 22:41:45 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.3-windowsservercore`

```console
$ docker pull nats@sha256:eb36b93a9338c371fb136c3966ea0b1d41c268eb78dcc3f0cf4b4e4e6dc2f924
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `nats:2.8.3-windowsservercore` - windows version 10.0.17763.2928; amd64

```console
$ docker pull nats@sha256:463326eba88d62c6de77af4874f4dea9ef53d30a6606dc475205c5444dd14c81
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2509545826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5404ddeeb235704c9be25463973cf8749998a527098877629130155ee1a8de6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Wed, 11 May 2022 12:42:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 May 2022 14:39:53 GMT
ENV NATS_DOCKERIZED=1
# Mon, 23 May 2022 22:14:24 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:14:24 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.3/nats-server-v2.8.3-windows-amd64.zip
# Mon, 23 May 2022 22:14:25 GMT
ENV NATS_SERVER_SHASUM=8195903f1d389327041ed50dddd62715b6aa74cc3f8f94865a8ae7b5875b3851
# Mon, 23 May 2022 22:15:24 GMT
RUN Set-PSDebug -Trace 2
# Mon, 23 May 2022 22:16:37 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 23 May 2022 22:16:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Mon, 23 May 2022 22:16:39 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:16:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 23 May 2022 22:16:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b34adcbd607b6c175a7c7a819fecbbfd53899678f53f169f2b4504070ec6b0ab`  
		Last Modified: Wed, 11 May 2022 14:07:06 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0c1e63aec5d8d83ee6bf4eb10d12ff30fe2e0eee737a2ef9291ead11cfb5cc`  
		Last Modified: Wed, 11 May 2022 14:42:43 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57b75a2edf35183ae898a9d68d8f5198163c53e5451d8da3b6a181ea8fa457f`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44a0c943278e9a6934267b495e21157256a8e0e59112d219700f1569327f153`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df2fa385bec1c86f1db9e768adf0323d7ae63afc30b2b61659eb4da17fc1412`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a33a8f0bf09b30dd9167b4150806163869b35f9c43ea15769b422ef5eaa919f`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 497.4 KB (497358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf09bb112173ae8d9e2df16abe56deb21191a622f289250dbc71ecff4b8faf3`  
		Last Modified: Mon, 23 May 2022 22:17:31 GMT  
		Size: 5.0 MB (4980200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e5cc1fbe4cfbdbdeceba96cd585d66515fb4ef8e79b738fb3cff04474e6f6d`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.8 KB (1846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600c2585823168fbd8f9f26a1dda94da2579919da1485501b17c799a1968a86c`  
		Last Modified: Mon, 23 May 2022 22:17:26 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3960c981235519da3181138ec9e48ef481177d8129cccc3620327e71a7c29860`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c546fa758ac26156e07083b8d1919a68568872dace58969c4714577dddfc1a3`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.8.3-windowsservercore-1809`

```console
$ docker pull nats@sha256:eb36b93a9338c371fb136c3966ea0b1d41c268eb78dcc3f0cf4b4e4e6dc2f924
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `nats:2.8.3-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull nats@sha256:463326eba88d62c6de77af4874f4dea9ef53d30a6606dc475205c5444dd14c81
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2509545826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5404ddeeb235704c9be25463973cf8749998a527098877629130155ee1a8de6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Wed, 11 May 2022 12:42:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 May 2022 14:39:53 GMT
ENV NATS_DOCKERIZED=1
# Mon, 23 May 2022 22:14:24 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:14:24 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.3/nats-server-v2.8.3-windows-amd64.zip
# Mon, 23 May 2022 22:14:25 GMT
ENV NATS_SERVER_SHASUM=8195903f1d389327041ed50dddd62715b6aa74cc3f8f94865a8ae7b5875b3851
# Mon, 23 May 2022 22:15:24 GMT
RUN Set-PSDebug -Trace 2
# Mon, 23 May 2022 22:16:37 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 23 May 2022 22:16:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Mon, 23 May 2022 22:16:39 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:16:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 23 May 2022 22:16:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b34adcbd607b6c175a7c7a819fecbbfd53899678f53f169f2b4504070ec6b0ab`  
		Last Modified: Wed, 11 May 2022 14:07:06 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0c1e63aec5d8d83ee6bf4eb10d12ff30fe2e0eee737a2ef9291ead11cfb5cc`  
		Last Modified: Wed, 11 May 2022 14:42:43 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57b75a2edf35183ae898a9d68d8f5198163c53e5451d8da3b6a181ea8fa457f`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44a0c943278e9a6934267b495e21157256a8e0e59112d219700f1569327f153`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df2fa385bec1c86f1db9e768adf0323d7ae63afc30b2b61659eb4da17fc1412`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a33a8f0bf09b30dd9167b4150806163869b35f9c43ea15769b422ef5eaa919f`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 497.4 KB (497358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf09bb112173ae8d9e2df16abe56deb21191a622f289250dbc71ecff4b8faf3`  
		Last Modified: Mon, 23 May 2022 22:17:31 GMT  
		Size: 5.0 MB (4980200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e5cc1fbe4cfbdbdeceba96cd585d66515fb4ef8e79b738fb3cff04474e6f6d`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.8 KB (1846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600c2585823168fbd8f9f26a1dda94da2579919da1485501b17c799a1968a86c`  
		Last Modified: Mon, 23 May 2022 22:17:26 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3960c981235519da3181138ec9e48ef481177d8129cccc3620327e71a7c29860`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c546fa758ac26156e07083b8d1919a68568872dace58969c4714577dddfc1a3`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:6052573e8a399a357cf0b7d84a694944aa016806d677a8026be807c56ce37354
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:2769de3270a9a86a1f799007cb1be2cbac229c07395206d13fbf845312481fc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7678717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0303f1d0cccc66a96da1353b9732b2b1b9dbd21206996b9af197b108e52d444b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 22:19:43 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:19:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 22:19:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 22:19:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 22:19:45 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:19:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 22:19:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68886d04807b30a327d175e97fe6fa560a6f4e68ea614397e87e7d456d6ace19`  
		Last Modified: Mon, 23 May 2022 22:20:18 GMT  
		Size: 4.9 MB (4863157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfc1bf8ce728acff89f87564fb40e67def44a450bd0e29f09309dad99e81ac6`  
		Last Modified: Mon, 23 May 2022 22:20:17 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c52785e040cd5cb0b784f0b7cf87f4ef40f0031383deb06acd3a5018bd0eee`  
		Last Modified: Mon, 23 May 2022 22:20:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:fcdca3dcbbb5b03284c64c0a9374301e1f7a901233a20a336949e932a510fd71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c863d799218e699e81cac4bbf925e850d19c0edf53ecabe58b02135444c6c01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 23:13:16 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 23:13:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 23:13:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 23:13:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 23:13:22 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 23:13:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 23:13:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b388d827d3aa697791f4a4d8097280f479f0faa6dc06e10f82c7653d34dcab`  
		Last Modified: Mon, 23 May 2022 23:15:27 GMT  
		Size: 4.5 MB (4518137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd801f49e3417e379c20c004c736e5b66baf62157ee6229ab1db746a0f665e46`  
		Last Modified: Mon, 23 May 2022 23:15:24 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877ff8ab778b23cf937adea367539b09513c39ed7e2af8f25a121793f7d0f68f`  
		Last Modified: Mon, 23 May 2022 23:15:24 GMT  
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
$ docker pull nats@sha256:adc4ca726f4e53b15e2a1d0d37aa7ff98c72bb2bd22fb72cac063d499b13bcba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7216231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f6313823af3524d1b2c8d4ce856935175e3ef55468eabfb142258efac8a00d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 22:40:07 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:40:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 22:40:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 22:40:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 22:40:12 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:40:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 22:40:14 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daa2cd1d5619c80b024c9f1d0980283c6ccd1a629a821540e044e4b1fdfcadf`  
		Last Modified: Mon, 23 May 2022 22:41:18 GMT  
		Size: 4.5 MB (4498780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ac0d288c25cbc55828b15cb671ae312a21835584b6c77e74cbd9513cb8813d`  
		Last Modified: Mon, 23 May 2022 22:41:17 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d9b1665dd8911a6f720bb3e6c144864b1907bd595f2141172a8a82bb0370ee`  
		Last Modified: Mon, 23 May 2022 22:41:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.15`

```console
$ docker pull nats@sha256:bb254c727e39b0b3b99244815bfa4144bbc5dc62df6c8a82d6bd6536788ccb91
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.15` - linux; amd64

```console
$ docker pull nats@sha256:2769de3270a9a86a1f799007cb1be2cbac229c07395206d13fbf845312481fc8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.7 MB (7678717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0303f1d0cccc66a96da1353b9732b2b1b9dbd21206996b9af197b108e52d444b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 22:19:43 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:19:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 22:19:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 22:19:45 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 22:19:45 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:19:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 22:19:45 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68886d04807b30a327d175e97fe6fa560a6f4e68ea614397e87e7d456d6ace19`  
		Last Modified: Mon, 23 May 2022 22:20:18 GMT  
		Size: 4.9 MB (4863157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfc1bf8ce728acff89f87564fb40e67def44a450bd0e29f09309dad99e81ac6`  
		Last Modified: Mon, 23 May 2022 22:20:17 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c52785e040cd5cb0b784f0b7cf87f4ef40f0031383deb06acd3a5018bd0eee`  
		Last Modified: Mon, 23 May 2022 22:20:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v6

```console
$ docker pull nats@sha256:fcdca3dcbbb5b03284c64c0a9374301e1f7a901233a20a336949e932a510fd71
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.1 MB (7141112 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c863d799218e699e81cac4bbf925e850d19c0edf53ecabe58b02135444c6c01`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 23:13:16 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 23:13:20 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 23:13:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 23:13:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 23:13:22 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 23:13:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 23:13:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b388d827d3aa697791f4a4d8097280f479f0faa6dc06e10f82c7653d34dcab`  
		Last Modified: Mon, 23 May 2022 23:15:27 GMT  
		Size: 4.5 MB (4518137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd801f49e3417e379c20c004c736e5b66baf62157ee6229ab1db746a0f665e46`  
		Last Modified: Mon, 23 May 2022 23:15:24 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877ff8ab778b23cf937adea367539b09513c39ed7e2af8f25a121793f7d0f68f`  
		Last Modified: Mon, 23 May 2022 23:15:24 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm variant v7

```console
$ docker pull nats@sha256:aa130a56f0b1428fc47e92102e4273d7cbff4b90534b8b134b2d658a6d1c38bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.9 MB (6938699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d68a57086629ed4e52dfa052c8b25706377fa32c9fb518fe4f8d3b74ba922f50`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 23:30:41 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 23:30:45 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 23:30:45 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 23:30:46 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 23:30:46 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 23:30:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 23:30:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a80fca66b8067494cea5416b87c794783f42324795d17be4972cfaed3c14c44`  
		Last Modified: Mon, 23 May 2022 23:32:55 GMT  
		Size: 4.5 MB (4513374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edf8c7c58b8c4cd539401a48d23026f9d28d2e99bad1997337a5cc45321f8873`  
		Last Modified: Mon, 23 May 2022 23:32:52 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a96a070c80e547148535de9946c1f98e6d8d8dfa7fe6ae1c51e269930f1e61`  
		Last Modified: Mon, 23 May 2022 23:32:52 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.15` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:adc4ca726f4e53b15e2a1d0d37aa7ff98c72bb2bd22fb72cac063d499b13bcba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.2 MB (7216231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f6313823af3524d1b2c8d4ce856935175e3ef55468eabfb142258efac8a00d1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Mon, 23 May 2022 22:40:07 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:40:09 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='905df5647dba0443ce6b92116ff5c6ceb49d3e24fa78c999d0c19fe634f341d6' ;; 		armhf) natsArch='arm6'; sha256='590a0460362ab1fc47ebce8886f5a53ff8b91abefa412ce77762f8514041394b' ;; 		armv7) natsArch='arm7'; sha256='142673f4eafca832e0347b1be0f5f9b0b7b23a46c08a623b63c6925a94a2d9f1' ;; 		x86_64) natsArch='amd64'; sha256='16e6bfa14e8ba9bc7d924e296bfe6bcad803b04318e6d60ef14ee45e3d3ddc60' ;; 		x86) natsArch='386'; sha256='fc749ab7574aa9ae22661a89ad73ac26331772e2302197d1625db56e967a74ac' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 23 May 2022 22:40:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 23 May 2022 22:40:12 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 23 May 2022 22:40:12 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:40:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 23 May 2022 22:40:14 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7daa2cd1d5619c80b024c9f1d0980283c6ccd1a629a821540e044e4b1fdfcadf`  
		Last Modified: Mon, 23 May 2022 22:41:18 GMT  
		Size: 4.5 MB (4498780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ac0d288c25cbc55828b15cb671ae312a21835584b6c77e74cbd9513cb8813d`  
		Last Modified: Mon, 23 May 2022 22:41:17 GMT  
		Size: 560.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d9b1665dd8911a6f720bb3e6c144864b1907bd595f2141172a8a82bb0370ee`  
		Last Modified: Mon, 23 May 2022 22:41:17 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:faf79ebeddcf0d20856df247744cdf519e8051a2480cb12b9f53c4c2e0086b3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2928; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:c4c5aa8d8b2ce861febd7bd4dcd9a729204ba3f15f91fd96f45ab5a6e100e516
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4590377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ca6ed6836bb8a2f8705608091864ce3c25b8ca32693003e2a8df04e30dc0f9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:19:51 GMT
COPY file:8ff89c4fbf2c06b0c443f547e21c09f4d00bc37565795d87bfb43a04d4ff236e in /nats-server 
# Mon, 23 May 2022 22:19:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:19:51 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:19:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:19:52 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:19:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:49229864ce5450b6b5291aa946e418a9b56e6bbac1179c2a3ca592284b674f6c`  
		Last Modified: Mon, 23 May 2022 22:20:42 GMT  
		Size: 4.6 MB (4589871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f11a75312c73ef42e06951cc5acd4b2690648b1ab001bacda9622a11819993`  
		Last Modified: Mon, 23 May 2022 22:20:41 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:0a83bd61fe2f1ebbf052ab13bd453c3dfaec1db3e86896718024aff558174bf9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea45afb007d73aa5822eb21ef9e9d34b90edd8cbb44379c26a50b550889c3d3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 23:13:43 GMT
COPY file:4121ba71c4705779a334ba22404be19aaa6e3e8946ec6b5ce733466627f8c88e in /nats-server 
# Mon, 23 May 2022 23:13:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 23:13:44 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 23:13:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 23:13:45 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 23:13:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3429a8151ae5ab692b14a1bd6742acff14f3fba53afc354782fbd5f6fc7b1421`  
		Last Modified: Mon, 23 May 2022 23:16:03 GMT  
		Size: 4.2 MB (4244908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251a42b41696b6a66317c2f99b1cd869dcdf07194f5f28e7edc10140fdf1acfd`  
		Last Modified: Mon, 23 May 2022 23:16:00 GMT  
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
$ docker pull nats@sha256:b368674b8858acdf4bdbb8bec04335cb6987fb1829159c212d781b689de74eea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4226009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2081876fa6098daea6a89b6894c8456c7b36939451c3d95d468ce493be85e1c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:40:25 GMT
COPY file:32e0c5d015acde93901500da0b0b479ba09cbb47d3918ad6d6b5523c686262ca in /nats-server 
# Mon, 23 May 2022 22:40:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:40:26 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:40:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:40:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:40:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7bdd5229d960e87b053609bd24bc82f46460a06899394029f599726df64da912`  
		Last Modified: Mon, 23 May 2022 22:41:46 GMT  
		Size: 4.2 MB (4225500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb661e40537a6e401894b3f7520bf397b6185ab575af1f5cf8bf40efcfd86bc`  
		Last Modified: Mon, 23 May 2022 22:41:45 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.2928; amd64

```console
$ docker pull nats@sha256:95b08fc423ab3d372702336dae5a8dbe2d1da429c18eeaf36f936fc0875ee7ac
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107772713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5d6c0f979e88d8401fee505a489498a7f206548060dfbf92e3adf4875a8ef8`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:42:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 23 May 2022 22:16:52 GMT
RUN cmd /S /C #(nop) COPY file:20c5da4e402adeb74e59df38a88afb7f0706725d1cf47a32deba2a95222bf05e in C:\nats-server.exe 
# Mon, 23 May 2022 22:16:53 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 23 May 2022 22:16:55 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2df39ac96d0b0efa546f2a05d81fb2a68ff8b0541fca6761bc2cedd28ff57f25`  
		Last Modified: Wed, 11 May 2022 14:43:01 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c75ab9a5e0f44e79c3adfc8b401bd352612bfa1c195e182dfedca24907fc2cb`  
		Last Modified: Mon, 23 May 2022 22:17:51 GMT  
		Size: 4.6 MB (4632778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7d580b9477c406ac03b52996e543c4d98651c583032c1cc8a15b97a42974d0`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.7 KB (1660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0c44352b5c88d59e36acd76446dfd0543670ed32caba214353a395b0e27590`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a07615e58e42c48f51d89c04072d98127ea7db787f97cdef0385b134fe681`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51272f4f628d52da760d5a41b2c254fe1082dbf88591529f520cc4d37a317a47`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:f29655b29b519414dd885e07d7d4bdf22055d39406af47961dae06def8c7c600
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:c4c5aa8d8b2ce861febd7bd4dcd9a729204ba3f15f91fd96f45ab5a6e100e516
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4590377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ca6ed6836bb8a2f8705608091864ce3c25b8ca32693003e2a8df04e30dc0f9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:19:51 GMT
COPY file:8ff89c4fbf2c06b0c443f547e21c09f4d00bc37565795d87bfb43a04d4ff236e in /nats-server 
# Mon, 23 May 2022 22:19:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:19:51 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:19:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:19:52 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:19:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:49229864ce5450b6b5291aa946e418a9b56e6bbac1179c2a3ca592284b674f6c`  
		Last Modified: Mon, 23 May 2022 22:20:42 GMT  
		Size: 4.6 MB (4589871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f11a75312c73ef42e06951cc5acd4b2690648b1ab001bacda9622a11819993`  
		Last Modified: Mon, 23 May 2022 22:20:41 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:0a83bd61fe2f1ebbf052ab13bd453c3dfaec1db3e86896718024aff558174bf9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea45afb007d73aa5822eb21ef9e9d34b90edd8cbb44379c26a50b550889c3d3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 23:13:43 GMT
COPY file:4121ba71c4705779a334ba22404be19aaa6e3e8946ec6b5ce733466627f8c88e in /nats-server 
# Mon, 23 May 2022 23:13:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 23:13:44 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 23:13:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 23:13:45 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 23:13:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3429a8151ae5ab692b14a1bd6742acff14f3fba53afc354782fbd5f6fc7b1421`  
		Last Modified: Mon, 23 May 2022 23:16:03 GMT  
		Size: 4.2 MB (4244908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251a42b41696b6a66317c2f99b1cd869dcdf07194f5f28e7edc10140fdf1acfd`  
		Last Modified: Mon, 23 May 2022 23:16:00 GMT  
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
$ docker pull nats@sha256:b368674b8858acdf4bdbb8bec04335cb6987fb1829159c212d781b689de74eea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4226009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2081876fa6098daea6a89b6894c8456c7b36939451c3d95d468ce493be85e1c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:40:25 GMT
COPY file:32e0c5d015acde93901500da0b0b479ba09cbb47d3918ad6d6b5523c686262ca in /nats-server 
# Mon, 23 May 2022 22:40:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:40:26 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:40:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:40:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:40:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7bdd5229d960e87b053609bd24bc82f46460a06899394029f599726df64da912`  
		Last Modified: Mon, 23 May 2022 22:41:46 GMT  
		Size: 4.2 MB (4225500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb661e40537a6e401894b3f7520bf397b6185ab575af1f5cf8bf40efcfd86bc`  
		Last Modified: Mon, 23 May 2022 22:41:45 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:f338915431c6f74ef7061f9d4349709e849edca4a9f6492c84cce0132a9219f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `nats:nanoserver` - windows version 10.0.17763.2928; amd64

```console
$ docker pull nats@sha256:95b08fc423ab3d372702336dae5a8dbe2d1da429c18eeaf36f936fc0875ee7ac
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107772713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5d6c0f979e88d8401fee505a489498a7f206548060dfbf92e3adf4875a8ef8`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:42:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 23 May 2022 22:16:52 GMT
RUN cmd /S /C #(nop) COPY file:20c5da4e402adeb74e59df38a88afb7f0706725d1cf47a32deba2a95222bf05e in C:\nats-server.exe 
# Mon, 23 May 2022 22:16:53 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 23 May 2022 22:16:55 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2df39ac96d0b0efa546f2a05d81fb2a68ff8b0541fca6761bc2cedd28ff57f25`  
		Last Modified: Wed, 11 May 2022 14:43:01 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c75ab9a5e0f44e79c3adfc8b401bd352612bfa1c195e182dfedca24907fc2cb`  
		Last Modified: Mon, 23 May 2022 22:17:51 GMT  
		Size: 4.6 MB (4632778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7d580b9477c406ac03b52996e543c4d98651c583032c1cc8a15b97a42974d0`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.7 KB (1660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0c44352b5c88d59e36acd76446dfd0543670ed32caba214353a395b0e27590`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a07615e58e42c48f51d89c04072d98127ea7db787f97cdef0385b134fe681`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51272f4f628d52da760d5a41b2c254fe1082dbf88591529f520cc4d37a317a47`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:f338915431c6f74ef7061f9d4349709e849edca4a9f6492c84cce0132a9219f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull nats@sha256:95b08fc423ab3d372702336dae5a8dbe2d1da429c18eeaf36f936fc0875ee7ac
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107772713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd5d6c0f979e88d8401fee505a489498a7f206548060dfbf92e3adf4875a8ef8`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 May 2022 16:42:43 GMT
RUN Apply image 10.0.17763.2928
# Wed, 11 May 2022 14:42:07 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 23 May 2022 22:16:52 GMT
RUN cmd /S /C #(nop) COPY file:20c5da4e402adeb74e59df38a88afb7f0706725d1cf47a32deba2a95222bf05e in C:\nats-server.exe 
# Mon, 23 May 2022 22:16:53 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:16:54 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 23 May 2022 22:16:55 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6626f490e738e10ea5e31ff2643e3a8c372e076d9030c77fac37537dbf12b73c`  
		Size: 103.1 MB (103133833 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2df39ac96d0b0efa546f2a05d81fb2a68ff8b0541fca6761bc2cedd28ff57f25`  
		Last Modified: Wed, 11 May 2022 14:43:01 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c75ab9a5e0f44e79c3adfc8b401bd352612bfa1c195e182dfedca24907fc2cb`  
		Last Modified: Mon, 23 May 2022 22:17:51 GMT  
		Size: 4.6 MB (4632778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e7d580b9477c406ac03b52996e543c4d98651c583032c1cc8a15b97a42974d0`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.7 KB (1660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0c44352b5c88d59e36acd76446dfd0543670ed32caba214353a395b0e27590`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:430a07615e58e42c48f51d89c04072d98127ea7db787f97cdef0385b134fe681`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51272f4f628d52da760d5a41b2c254fe1082dbf88591529f520cc4d37a317a47`  
		Last Modified: Mon, 23 May 2022 22:17:46 GMT  
		Size: 1.1 KB (1061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:f29655b29b519414dd885e07d7d4bdf22055d39406af47961dae06def8c7c600
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:c4c5aa8d8b2ce861febd7bd4dcd9a729204ba3f15f91fd96f45ab5a6e100e516
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4590377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1ca6ed6836bb8a2f8705608091864ce3c25b8ca32693003e2a8df04e30dc0f9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:19:51 GMT
COPY file:8ff89c4fbf2c06b0c443f547e21c09f4d00bc37565795d87bfb43a04d4ff236e in /nats-server 
# Mon, 23 May 2022 22:19:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:19:51 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:19:52 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:19:52 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:19:52 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:49229864ce5450b6b5291aa946e418a9b56e6bbac1179c2a3ca592284b674f6c`  
		Last Modified: Mon, 23 May 2022 22:20:42 GMT  
		Size: 4.6 MB (4589871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92f11a75312c73ef42e06951cc5acd4b2690648b1ab001bacda9622a11819993`  
		Last Modified: Mon, 23 May 2022 22:20:41 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:0a83bd61fe2f1ebbf052ab13bd453c3dfaec1db3e86896718024aff558174bf9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea45afb007d73aa5822eb21ef9e9d34b90edd8cbb44379c26a50b550889c3d3c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 23:13:43 GMT
COPY file:4121ba71c4705779a334ba22404be19aaa6e3e8946ec6b5ce733466627f8c88e in /nats-server 
# Mon, 23 May 2022 23:13:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 23:13:44 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 23:13:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 23:13:45 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 23:13:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3429a8151ae5ab692b14a1bd6742acff14f3fba53afc354782fbd5f6fc7b1421`  
		Last Modified: Mon, 23 May 2022 23:16:03 GMT  
		Size: 4.2 MB (4244908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251a42b41696b6a66317c2f99b1cd869dcdf07194f5f28e7edc10140fdf1acfd`  
		Last Modified: Mon, 23 May 2022 23:16:00 GMT  
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
$ docker pull nats@sha256:b368674b8858acdf4bdbb8bec04335cb6987fb1829159c212d781b689de74eea
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4226009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2081876fa6098daea6a89b6894c8456c7b36939451c3d95d468ce493be85e1c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 23 May 2022 22:40:25 GMT
COPY file:32e0c5d015acde93901500da0b0b479ba09cbb47d3918ad6d6b5523c686262ca in /nats-server 
# Mon, 23 May 2022 22:40:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 23 May 2022 22:40:26 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:40:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 23 May 2022 22:40:28 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 23 May 2022 22:40:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:7bdd5229d960e87b053609bd24bc82f46460a06899394029f599726df64da912`  
		Last Modified: Mon, 23 May 2022 22:41:46 GMT  
		Size: 4.2 MB (4225500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb661e40537a6e401894b3f7520bf397b6185ab575af1f5cf8bf40efcfd86bc`  
		Last Modified: Mon, 23 May 2022 22:41:45 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:eb36b93a9338c371fb136c3966ea0b1d41c268eb78dcc3f0cf4b4e4e6dc2f924
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `nats:windowsservercore` - windows version 10.0.17763.2928; amd64

```console
$ docker pull nats@sha256:463326eba88d62c6de77af4874f4dea9ef53d30a6606dc475205c5444dd14c81
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2509545826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5404ddeeb235704c9be25463973cf8749998a527098877629130155ee1a8de6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Wed, 11 May 2022 12:42:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 May 2022 14:39:53 GMT
ENV NATS_DOCKERIZED=1
# Mon, 23 May 2022 22:14:24 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:14:24 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.3/nats-server-v2.8.3-windows-amd64.zip
# Mon, 23 May 2022 22:14:25 GMT
ENV NATS_SERVER_SHASUM=8195903f1d389327041ed50dddd62715b6aa74cc3f8f94865a8ae7b5875b3851
# Mon, 23 May 2022 22:15:24 GMT
RUN Set-PSDebug -Trace 2
# Mon, 23 May 2022 22:16:37 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 23 May 2022 22:16:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Mon, 23 May 2022 22:16:39 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:16:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 23 May 2022 22:16:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b34adcbd607b6c175a7c7a819fecbbfd53899678f53f169f2b4504070ec6b0ab`  
		Last Modified: Wed, 11 May 2022 14:07:06 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0c1e63aec5d8d83ee6bf4eb10d12ff30fe2e0eee737a2ef9291ead11cfb5cc`  
		Last Modified: Wed, 11 May 2022 14:42:43 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57b75a2edf35183ae898a9d68d8f5198163c53e5451d8da3b6a181ea8fa457f`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44a0c943278e9a6934267b495e21157256a8e0e59112d219700f1569327f153`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df2fa385bec1c86f1db9e768adf0323d7ae63afc30b2b61659eb4da17fc1412`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a33a8f0bf09b30dd9167b4150806163869b35f9c43ea15769b422ef5eaa919f`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 497.4 KB (497358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf09bb112173ae8d9e2df16abe56deb21191a622f289250dbc71ecff4b8faf3`  
		Last Modified: Mon, 23 May 2022 22:17:31 GMT  
		Size: 5.0 MB (4980200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e5cc1fbe4cfbdbdeceba96cd585d66515fb4ef8e79b738fb3cff04474e6f6d`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.8 KB (1846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600c2585823168fbd8f9f26a1dda94da2579919da1485501b17c799a1968a86c`  
		Last Modified: Mon, 23 May 2022 22:17:26 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3960c981235519da3181138ec9e48ef481177d8129cccc3620327e71a7c29860`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c546fa758ac26156e07083b8d1919a68568872dace58969c4714577dddfc1a3`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:eb36b93a9338c371fb136c3966ea0b1d41c268eb78dcc3f0cf4b4e4e6dc2f924
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull nats@sha256:463326eba88d62c6de77af4874f4dea9ef53d30a6606dc475205c5444dd14c81
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2509545826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5404ddeeb235704c9be25463973cf8749998a527098877629130155ee1a8de6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Wed, 11 May 2022 12:42:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 May 2022 14:39:53 GMT
ENV NATS_DOCKERIZED=1
# Mon, 23 May 2022 22:14:24 GMT
ENV NATS_SERVER=2.8.3
# Mon, 23 May 2022 22:14:24 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.8.3/nats-server-v2.8.3-windows-amd64.zip
# Mon, 23 May 2022 22:14:25 GMT
ENV NATS_SERVER_SHASUM=8195903f1d389327041ed50dddd62715b6aa74cc3f8f94865a8ae7b5875b3851
# Mon, 23 May 2022 22:15:24 GMT
RUN Set-PSDebug -Trace 2
# Mon, 23 May 2022 22:16:37 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Mon, 23 May 2022 22:16:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Mon, 23 May 2022 22:16:39 GMT
EXPOSE 4222 6222 8222
# Mon, 23 May 2022 22:16:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Mon, 23 May 2022 22:16:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b34adcbd607b6c175a7c7a819fecbbfd53899678f53f169f2b4504070ec6b0ab`  
		Last Modified: Wed, 11 May 2022 14:07:06 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0c1e63aec5d8d83ee6bf4eb10d12ff30fe2e0eee737a2ef9291ead11cfb5cc`  
		Last Modified: Wed, 11 May 2022 14:42:43 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57b75a2edf35183ae898a9d68d8f5198163c53e5451d8da3b6a181ea8fa457f`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44a0c943278e9a6934267b495e21157256a8e0e59112d219700f1569327f153`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df2fa385bec1c86f1db9e768adf0323d7ae63afc30b2b61659eb4da17fc1412`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a33a8f0bf09b30dd9167b4150806163869b35f9c43ea15769b422ef5eaa919f`  
		Last Modified: Mon, 23 May 2022 22:17:28 GMT  
		Size: 497.4 KB (497358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf09bb112173ae8d9e2df16abe56deb21191a622f289250dbc71ecff4b8faf3`  
		Last Modified: Mon, 23 May 2022 22:17:31 GMT  
		Size: 5.0 MB (4980200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e5cc1fbe4cfbdbdeceba96cd585d66515fb4ef8e79b738fb3cff04474e6f6d`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.8 KB (1846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600c2585823168fbd8f9f26a1dda94da2579919da1485501b17c799a1968a86c`  
		Last Modified: Mon, 23 May 2022 22:17:26 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3960c981235519da3181138ec9e48ef481177d8129cccc3620327e71a7c29860`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c546fa758ac26156e07083b8d1919a68568872dace58969c4714577dddfc1a3`  
		Last Modified: Mon, 23 May 2022 22:17:25 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
