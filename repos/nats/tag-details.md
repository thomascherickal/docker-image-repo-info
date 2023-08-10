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
-	[`nats:2.9.21`](#nats2921)
-	[`nats:2.9.21-alpine`](#nats2921-alpine)
-	[`nats:2.9.21-alpine3.18`](#nats2921-alpine318)
-	[`nats:2.9.21-linux`](#nats2921-linux)
-	[`nats:2.9.21-nanoserver`](#nats2921-nanoserver)
-	[`nats:2.9.21-nanoserver-1809`](#nats2921-nanoserver-1809)
-	[`nats:2.9.21-scratch`](#nats2921-scratch)
-	[`nats:2.9.21-windowsservercore`](#nats2921-windowsservercore)
-	[`nats:2.9.21-windowsservercore-1809`](#nats2921-windowsservercore-1809)
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
$ docker pull nats@sha256:a75b6817e3135f1f789e970a62980e49b9efa3d3cdfc7db4193312f12cb44b3f
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
$ docker pull nats@sha256:cf96338e314ee46e307626e8936dc31b9ef7c67e299b29b7753896d11b52fe8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5455cadbb1bd4919947f5a918491add0f2a8fe5d9aa4a801ca79a4ac8fb308f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:26:10 GMT
COPY file:975a38b1520c81a5e1d0876325548b4aefe0036b6deee1ae7ee20db6abbcc080 in /nats-server 
# Mon, 07 Aug 2023 19:26:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:26:11 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:26:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:26:11 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:26:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc02d5ba29398595681917073dcd141022b8ad8d0da9a18b6f5752e56c86ceea`  
		Last Modified: Mon, 07 Aug 2023 19:26:56 GMT  
		Size: 5.2 MB (5169747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9457cd0af5e7125dfe4a44e1d6d003e2bdaf42da9d1c5f7b313069a145e639`  
		Last Modified: Mon, 07 Aug 2023 19:26:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v6

```console
$ docker pull nats@sha256:3a3792aaaf193e57879f3594e95501c1372bd2a537965db2bc68fd85c13b8cb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4932529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966d4a644152a12918ae66827a94561e477b28d10bd2698612566a5c989612f1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:447be8988a65ae095af689a396d155107ebc910fe545508c6e6af6f1c2d2c4d4 in /nats-server 
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:50:31 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:50:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:50:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:50:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:590d3f4a49d783a9889465cc7862cf43dc4d3a60e0fb075544618efee1ef93e1`  
		Last Modified: Mon, 07 Aug 2023 19:51:13 GMT  
		Size: 4.9 MB (4932022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901e46e20099bb53f1d1b41e9f1cbf04d9af77173e45873723bd9d7825fbbcf0`  
		Last Modified: Mon, 07 Aug 2023 19:51:12 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm variant v7

```console
$ docker pull nats@sha256:3be04f93d99a8e23e99fff2608d9c0d76a4ee2c9c301441f57a2d0b9225c16e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4924573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec722342be0e9d946cb8ac26674a30ff2854116e2e8e1ba75461b3f90d97ecc8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:a28d4beb7d3acaa71be2e58ce3a707a2f5be041842f8a1e4eb4c54dd72e865eb in /nats-server 
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 20:16:33 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 20:16:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 20:16:33 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 20:16:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:68043f4483bff82380b8666c025686881f5483ff754784192f65aa4ec9b662fe`  
		Last Modified: Mon, 07 Aug 2023 20:17:27 GMT  
		Size: 4.9 MB (4924065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0443d8f0ff2c43f481bd49043e2c13423203b3a99754a3baff7df20850bf0e56`  
		Last Modified: Mon, 07 Aug 2023 20:17:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24cb726cdaa647f5307f6d5fa448b299535141c96367b79636f23597407b5071
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4734399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b2f013bc2559b3a905b049fd4b09738b17a4c87d62bed5a1830c6a6e13b1cda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:815b9c4a7d715138f02171cd656c9e8dc6d80e72107c92661c99f6dd24ae2721 in /nats-server 
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:44:14 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:44:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:44:14 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:44:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07116324214b64589e3a471932fe7f6b892068a7cd9cf9bb72a8ea25f8a92200`  
		Last Modified: Mon, 07 Aug 2023 19:44:57 GMT  
		Size: 4.7 MB (4733893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615975e7d25e46607f561d13c4c244d070bb41701a0ac2103df98dcb33e8a4eb`  
		Last Modified: Mon, 07 Aug 2023 19:44:56 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:d8a94368172a3df5204943029b32d7b56dda869dadef4983129598ed86fcec67
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109707647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b1b071e5cf657d3db4c3347053329658550fdb8b09ae38a2618af5b119a8565`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 10 Aug 2023 02:34:53 GMT
RUN cmd /S /C #(nop) COPY file:3b8a3a4f656cc66920d77ff06f41851caa37056073cec32caf7e7024bea62100 in C:\nats-server.exe 
# Thu, 10 Aug 2023 02:34:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 10 Aug 2023 02:34:56 GMT
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
	-	`sha256:6810a6f695e6275423db76be5637667297faaa666b58a9658e1690efe300b007`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 5.2 MB (5242246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fbe96bd125f3ebe2f71079f2d8c4ca1d226d4aa3de1dd2a0fefb0e50421464`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c6c360e7d8fa0f4858a220d96a5d13e7c65c195bb8513191b47c1d3b0c6b91`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3db71fcfd8d9cd70e2947e60d0f27dee2449c365fcd7dde18997017f1f7a443`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112aff03752bdfd32ed33505dc8c488a27bdc249bd506edd30af3d47c0d9b4a2`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:511f5c4cfc6fdd61eb66afab99dfb38bed69aae630d8d5b36bc9bfc716723cd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:5cf5c3802d1e857d169a3f1d5cbe4799d4839fd6f55af788cedcb6e5a22378e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9195249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4997d3c6db9cae525d31602ba338a453ba4facd93e802fa29b3ba534475bd9f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:26:02 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:26:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:26:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:26:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:26:05 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:26:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:26:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd25bdbc8b4e243f7c3ffdffcc8115824b4b4cb2e9e73e3daadb257d79643d2`  
		Last Modified: Mon, 07 Aug 2023 19:26:33 GMT  
		Size: 5.8 MB (5792639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115edb875772e3386f7d2813cc6497fbdbaea0f7f9a39e552e3309472365aa90`  
		Last Modified: Mon, 07 Aug 2023 19:26:32 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279c31eb6dadb7f2e0ca227988e36fd0206af24465e2a207d488967470b3a63e`  
		Last Modified: Mon, 07 Aug 2023 19:26:32 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:5e07de3c322c8771519734bef7e466ac5028ab54275802d4deb77c36411e3cbb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8700810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e0fee524fb6e7f519b9ae3abd80976c1836c3f10c0be79daf8e035556935b24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:50:24 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:50:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:50:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:50:28 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:50:28 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:50:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:50:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee480b732706005fa701c3c4028a724e52a4fae0fd1c0aa66e0c837002d561d`  
		Last Modified: Mon, 07 Aug 2023 19:50:50 GMT  
		Size: 5.6 MB (5555005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58f30a3786b4a2dc69c83b465d31a4f645160b79da0a61c29860cdc3972b214`  
		Last Modified: Mon, 07 Aug 2023 19:50:49 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e541018b825fe9c407a093e7cac7a09742ba147db4c9b701c8021337ff70ec`  
		Last Modified: Mon, 07 Aug 2023 19:50:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:c4769e1e475367da9b4fc5a660a6fb32b200d27a3d026495fdc5bf74f9388c16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8447620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9893408047cef17e55311c80520a2cceb027a6e9d68f7206dc77b1330526c23e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:16:18 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 20:16:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 20:16:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 20:16:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 20:16:22 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 20:16:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:16:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fca2c62cfb95a8e21097e5398887f17729f82e97f22aba05b4a501ead7235bf`  
		Last Modified: Mon, 07 Aug 2023 20:17:02 GMT  
		Size: 5.5 MB (5547144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c778dd55b3c0df3d1fa0c07a38398ecd9605779c83aad61a071e63327b6077a`  
		Last Modified: Mon, 07 Aug 2023 20:17:00 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f262374e9fca7560e610908419255255f99f7ce00698f5da57b988be8a0827`  
		Last Modified: Mon, 07 Aug 2023 20:17:00 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:280523d3cd269840cf3ca0436eaf836b84057947803f07af5208ef8b7a1f765f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8689649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b733a68b85bf5e9f179e1363356f48edd81ae5fe656cf38413a97a99945327f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:44:08 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:44:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:44:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:44:10 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:44:10 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:44:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:44:10 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7eb0af764262eda43da676eb6212706a1a5c91fc0745feec3c2a78b11feeb74`  
		Last Modified: Mon, 07 Aug 2023 19:44:35 GMT  
		Size: 5.4 MB (5357887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d47d30642d18189ee8bcbc7387c01d1eddb910a0927366bf969f74ba950073`  
		Last Modified: Mon, 07 Aug 2023 19:44:34 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ace711cbe0f8fc6e880cdb92d235a3031e40977634be3a9fe209f05e65a7b7`  
		Last Modified: Mon, 07 Aug 2023 19:44:34 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.18`

```console
$ docker pull nats@sha256:511f5c4cfc6fdd61eb66afab99dfb38bed69aae630d8d5b36bc9bfc716723cd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:5cf5c3802d1e857d169a3f1d5cbe4799d4839fd6f55af788cedcb6e5a22378e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9195249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4997d3c6db9cae525d31602ba338a453ba4facd93e802fa29b3ba534475bd9f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:26:02 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:26:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:26:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:26:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:26:05 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:26:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:26:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd25bdbc8b4e243f7c3ffdffcc8115824b4b4cb2e9e73e3daadb257d79643d2`  
		Last Modified: Mon, 07 Aug 2023 19:26:33 GMT  
		Size: 5.8 MB (5792639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115edb875772e3386f7d2813cc6497fbdbaea0f7f9a39e552e3309472365aa90`  
		Last Modified: Mon, 07 Aug 2023 19:26:32 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279c31eb6dadb7f2e0ca227988e36fd0206af24465e2a207d488967470b3a63e`  
		Last Modified: Mon, 07 Aug 2023 19:26:32 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:5e07de3c322c8771519734bef7e466ac5028ab54275802d4deb77c36411e3cbb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8700810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e0fee524fb6e7f519b9ae3abd80976c1836c3f10c0be79daf8e035556935b24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:50:24 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:50:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:50:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:50:28 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:50:28 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:50:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:50:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee480b732706005fa701c3c4028a724e52a4fae0fd1c0aa66e0c837002d561d`  
		Last Modified: Mon, 07 Aug 2023 19:50:50 GMT  
		Size: 5.6 MB (5555005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58f30a3786b4a2dc69c83b465d31a4f645160b79da0a61c29860cdc3972b214`  
		Last Modified: Mon, 07 Aug 2023 19:50:49 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e541018b825fe9c407a093e7cac7a09742ba147db4c9b701c8021337ff70ec`  
		Last Modified: Mon, 07 Aug 2023 19:50:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:c4769e1e475367da9b4fc5a660a6fb32b200d27a3d026495fdc5bf74f9388c16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8447620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9893408047cef17e55311c80520a2cceb027a6e9d68f7206dc77b1330526c23e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:16:18 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 20:16:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 20:16:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 20:16:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 20:16:22 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 20:16:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:16:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fca2c62cfb95a8e21097e5398887f17729f82e97f22aba05b4a501ead7235bf`  
		Last Modified: Mon, 07 Aug 2023 20:17:02 GMT  
		Size: 5.5 MB (5547144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c778dd55b3c0df3d1fa0c07a38398ecd9605779c83aad61a071e63327b6077a`  
		Last Modified: Mon, 07 Aug 2023 20:17:00 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f262374e9fca7560e610908419255255f99f7ce00698f5da57b988be8a0827`  
		Last Modified: Mon, 07 Aug 2023 20:17:00 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:280523d3cd269840cf3ca0436eaf836b84057947803f07af5208ef8b7a1f765f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8689649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b733a68b85bf5e9f179e1363356f48edd81ae5fe656cf38413a97a99945327f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:44:08 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:44:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:44:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:44:10 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:44:10 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:44:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:44:10 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7eb0af764262eda43da676eb6212706a1a5c91fc0745feec3c2a78b11feeb74`  
		Last Modified: Mon, 07 Aug 2023 19:44:35 GMT  
		Size: 5.4 MB (5357887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d47d30642d18189ee8bcbc7387c01d1eddb910a0927366bf969f74ba950073`  
		Last Modified: Mon, 07 Aug 2023 19:44:34 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ace711cbe0f8fc6e880cdb92d235a3031e40977634be3a9fe209f05e65a7b7`  
		Last Modified: Mon, 07 Aug 2023 19:44:34 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:3208778cf6c64114c84d0227bfd6fb282f1ba86b85f25c46c410c9e97b3a33ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:cf96338e314ee46e307626e8936dc31b9ef7c67e299b29b7753896d11b52fe8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5455cadbb1bd4919947f5a918491add0f2a8fe5d9aa4a801ca79a4ac8fb308f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:26:10 GMT
COPY file:975a38b1520c81a5e1d0876325548b4aefe0036b6deee1ae7ee20db6abbcc080 in /nats-server 
# Mon, 07 Aug 2023 19:26:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:26:11 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:26:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:26:11 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:26:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc02d5ba29398595681917073dcd141022b8ad8d0da9a18b6f5752e56c86ceea`  
		Last Modified: Mon, 07 Aug 2023 19:26:56 GMT  
		Size: 5.2 MB (5169747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9457cd0af5e7125dfe4a44e1d6d003e2bdaf42da9d1c5f7b313069a145e639`  
		Last Modified: Mon, 07 Aug 2023 19:26:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:3a3792aaaf193e57879f3594e95501c1372bd2a537965db2bc68fd85c13b8cb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4932529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966d4a644152a12918ae66827a94561e477b28d10bd2698612566a5c989612f1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:447be8988a65ae095af689a396d155107ebc910fe545508c6e6af6f1c2d2c4d4 in /nats-server 
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:50:31 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:50:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:50:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:50:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:590d3f4a49d783a9889465cc7862cf43dc4d3a60e0fb075544618efee1ef93e1`  
		Last Modified: Mon, 07 Aug 2023 19:51:13 GMT  
		Size: 4.9 MB (4932022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901e46e20099bb53f1d1b41e9f1cbf04d9af77173e45873723bd9d7825fbbcf0`  
		Last Modified: Mon, 07 Aug 2023 19:51:12 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:3be04f93d99a8e23e99fff2608d9c0d76a4ee2c9c301441f57a2d0b9225c16e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4924573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec722342be0e9d946cb8ac26674a30ff2854116e2e8e1ba75461b3f90d97ecc8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:a28d4beb7d3acaa71be2e58ce3a707a2f5be041842f8a1e4eb4c54dd72e865eb in /nats-server 
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 20:16:33 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 20:16:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 20:16:33 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 20:16:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:68043f4483bff82380b8666c025686881f5483ff754784192f65aa4ec9b662fe`  
		Last Modified: Mon, 07 Aug 2023 20:17:27 GMT  
		Size: 4.9 MB (4924065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0443d8f0ff2c43f481bd49043e2c13423203b3a99754a3baff7df20850bf0e56`  
		Last Modified: Mon, 07 Aug 2023 20:17:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24cb726cdaa647f5307f6d5fa448b299535141c96367b79636f23597407b5071
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4734399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b2f013bc2559b3a905b049fd4b09738b17a4c87d62bed5a1830c6a6e13b1cda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:815b9c4a7d715138f02171cd656c9e8dc6d80e72107c92661c99f6dd24ae2721 in /nats-server 
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:44:14 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:44:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:44:14 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:44:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07116324214b64589e3a471932fe7f6b892068a7cd9cf9bb72a8ea25f8a92200`  
		Last Modified: Mon, 07 Aug 2023 19:44:57 GMT  
		Size: 4.7 MB (4733893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615975e7d25e46607f561d13c4c244d070bb41701a0ac2103df98dcb33e8a4eb`  
		Last Modified: Mon, 07 Aug 2023 19:44:56 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:3959865fd1e3f0b07b7933b6e4772490b619811c09074cfe6fd00985b6614f83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:d8a94368172a3df5204943029b32d7b56dda869dadef4983129598ed86fcec67
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109707647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b1b071e5cf657d3db4c3347053329658550fdb8b09ae38a2618af5b119a8565`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 10 Aug 2023 02:34:53 GMT
RUN cmd /S /C #(nop) COPY file:3b8a3a4f656cc66920d77ff06f41851caa37056073cec32caf7e7024bea62100 in C:\nats-server.exe 
# Thu, 10 Aug 2023 02:34:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 10 Aug 2023 02:34:56 GMT
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
	-	`sha256:6810a6f695e6275423db76be5637667297faaa666b58a9658e1690efe300b007`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 5.2 MB (5242246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fbe96bd125f3ebe2f71079f2d8c4ca1d226d4aa3de1dd2a0fefb0e50421464`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c6c360e7d8fa0f4858a220d96a5d13e7c65c195bb8513191b47c1d3b0c6b91`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3db71fcfd8d9cd70e2947e60d0f27dee2449c365fcd7dde18997017f1f7a443`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112aff03752bdfd32ed33505dc8c488a27bdc249bd506edd30af3d47c0d9b4a2`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:3959865fd1e3f0b07b7933b6e4772490b619811c09074cfe6fd00985b6614f83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:d8a94368172a3df5204943029b32d7b56dda869dadef4983129598ed86fcec67
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109707647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b1b071e5cf657d3db4c3347053329658550fdb8b09ae38a2618af5b119a8565`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 10 Aug 2023 02:34:53 GMT
RUN cmd /S /C #(nop) COPY file:3b8a3a4f656cc66920d77ff06f41851caa37056073cec32caf7e7024bea62100 in C:\nats-server.exe 
# Thu, 10 Aug 2023 02:34:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 10 Aug 2023 02:34:56 GMT
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
	-	`sha256:6810a6f695e6275423db76be5637667297faaa666b58a9658e1690efe300b007`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 5.2 MB (5242246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fbe96bd125f3ebe2f71079f2d8c4ca1d226d4aa3de1dd2a0fefb0e50421464`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c6c360e7d8fa0f4858a220d96a5d13e7c65c195bb8513191b47c1d3b0c6b91`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3db71fcfd8d9cd70e2947e60d0f27dee2449c365fcd7dde18997017f1f7a443`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112aff03752bdfd32ed33505dc8c488a27bdc249bd506edd30af3d47c0d9b4a2`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:3208778cf6c64114c84d0227bfd6fb282f1ba86b85f25c46c410c9e97b3a33ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:cf96338e314ee46e307626e8936dc31b9ef7c67e299b29b7753896d11b52fe8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5455cadbb1bd4919947f5a918491add0f2a8fe5d9aa4a801ca79a4ac8fb308f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:26:10 GMT
COPY file:975a38b1520c81a5e1d0876325548b4aefe0036b6deee1ae7ee20db6abbcc080 in /nats-server 
# Mon, 07 Aug 2023 19:26:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:26:11 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:26:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:26:11 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:26:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc02d5ba29398595681917073dcd141022b8ad8d0da9a18b6f5752e56c86ceea`  
		Last Modified: Mon, 07 Aug 2023 19:26:56 GMT  
		Size: 5.2 MB (5169747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9457cd0af5e7125dfe4a44e1d6d003e2bdaf42da9d1c5f7b313069a145e639`  
		Last Modified: Mon, 07 Aug 2023 19:26:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:3a3792aaaf193e57879f3594e95501c1372bd2a537965db2bc68fd85c13b8cb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4932529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966d4a644152a12918ae66827a94561e477b28d10bd2698612566a5c989612f1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:447be8988a65ae095af689a396d155107ebc910fe545508c6e6af6f1c2d2c4d4 in /nats-server 
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:50:31 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:50:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:50:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:50:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:590d3f4a49d783a9889465cc7862cf43dc4d3a60e0fb075544618efee1ef93e1`  
		Last Modified: Mon, 07 Aug 2023 19:51:13 GMT  
		Size: 4.9 MB (4932022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901e46e20099bb53f1d1b41e9f1cbf04d9af77173e45873723bd9d7825fbbcf0`  
		Last Modified: Mon, 07 Aug 2023 19:51:12 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:3be04f93d99a8e23e99fff2608d9c0d76a4ee2c9c301441f57a2d0b9225c16e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4924573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec722342be0e9d946cb8ac26674a30ff2854116e2e8e1ba75461b3f90d97ecc8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:a28d4beb7d3acaa71be2e58ce3a707a2f5be041842f8a1e4eb4c54dd72e865eb in /nats-server 
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 20:16:33 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 20:16:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 20:16:33 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 20:16:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:68043f4483bff82380b8666c025686881f5483ff754784192f65aa4ec9b662fe`  
		Last Modified: Mon, 07 Aug 2023 20:17:27 GMT  
		Size: 4.9 MB (4924065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0443d8f0ff2c43f481bd49043e2c13423203b3a99754a3baff7df20850bf0e56`  
		Last Modified: Mon, 07 Aug 2023 20:17:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24cb726cdaa647f5307f6d5fa448b299535141c96367b79636f23597407b5071
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4734399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b2f013bc2559b3a905b049fd4b09738b17a4c87d62bed5a1830c6a6e13b1cda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:815b9c4a7d715138f02171cd656c9e8dc6d80e72107c92661c99f6dd24ae2721 in /nats-server 
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:44:14 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:44:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:44:14 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:44:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07116324214b64589e3a471932fe7f6b892068a7cd9cf9bb72a8ea25f8a92200`  
		Last Modified: Mon, 07 Aug 2023 19:44:57 GMT  
		Size: 4.7 MB (4733893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615975e7d25e46607f561d13c4c244d070bb41701a0ac2103df98dcb33e8a4eb`  
		Last Modified: Mon, 07 Aug 2023 19:44:56 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:6a5048505a376ddee83a546a4c677bd2c62eaf943530ea64bc946e77b092500c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:df85f652123fd850bc088bf1796ad63e262c83117ef33c913c2324c329e83281
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2001923911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba49e1850a02235e7b24a350ba3483aa40adb3e25011cf8af425be0f74d9bb21`
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
# Thu, 10 Aug 2023 02:32:09 GMT
ENV NATS_SERVER=2.9.21
# Thu, 10 Aug 2023 02:32:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.21/nats-server-v2.9.21-windows-amd64.zip
# Thu, 10 Aug 2023 02:32:11 GMT
ENV NATS_SERVER_SHASUM=43df40bcf81e819e3467a31c548643439d4200486f3032c61ae4b134243f8796
# Thu, 10 Aug 2023 02:33:09 GMT
RUN Set-PSDebug -Trace 2
# Thu, 10 Aug 2023 02:34:42 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 10 Aug 2023 02:34:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 10 Aug 2023 02:34:44 GMT
EXPOSE 4222 6222 8222
# Thu, 10 Aug 2023 02:34:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 10 Aug 2023 02:34:45 GMT
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
	-	`sha256:8065a1cb0e804bbb19260f95fcb2ee724ea73de1da4df8e9744f6498cec33d62`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5638bc45d3356ae277d06dab7b839bf52e16bc50a37408b0de976cebfcd1ab`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc44a5e39ba10538d5f0af74a7c7c00bb731116d9f5f8f19b9469e2464baf901`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98483cb493b32b2587f35850b72b5beb7a5354034943519da2056a8b88a51036`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 242.8 KB (242767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7678609a7e25485895fffda9b5eea9f940ffc5e5e34155de64f2933803428c0e`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 5.7 MB (5712861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b6362b379d0e5ed852e577058ae198521bd47c70a6654e5bdd24a5fbc7f326`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79936c5c24a0ca205db9a615d4c0113a2e3093ae64cdabc9a8b1fa930327830c`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca71b03ad3cfece28d778d224d9c61ca3dbea97dc6761af0d411ddb0275f965d`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484f29887b314709fa52867baf4fc140ec7488361c38d1811854c07d682c1451`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:6a5048505a376ddee83a546a4c677bd2c62eaf943530ea64bc946e77b092500c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:df85f652123fd850bc088bf1796ad63e262c83117ef33c913c2324c329e83281
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2001923911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba49e1850a02235e7b24a350ba3483aa40adb3e25011cf8af425be0f74d9bb21`
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
# Thu, 10 Aug 2023 02:32:09 GMT
ENV NATS_SERVER=2.9.21
# Thu, 10 Aug 2023 02:32:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.21/nats-server-v2.9.21-windows-amd64.zip
# Thu, 10 Aug 2023 02:32:11 GMT
ENV NATS_SERVER_SHASUM=43df40bcf81e819e3467a31c548643439d4200486f3032c61ae4b134243f8796
# Thu, 10 Aug 2023 02:33:09 GMT
RUN Set-PSDebug -Trace 2
# Thu, 10 Aug 2023 02:34:42 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 10 Aug 2023 02:34:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 10 Aug 2023 02:34:44 GMT
EXPOSE 4222 6222 8222
# Thu, 10 Aug 2023 02:34:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 10 Aug 2023 02:34:45 GMT
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
	-	`sha256:8065a1cb0e804bbb19260f95fcb2ee724ea73de1da4df8e9744f6498cec33d62`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5638bc45d3356ae277d06dab7b839bf52e16bc50a37408b0de976cebfcd1ab`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc44a5e39ba10538d5f0af74a7c7c00bb731116d9f5f8f19b9469e2464baf901`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98483cb493b32b2587f35850b72b5beb7a5354034943519da2056a8b88a51036`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 242.8 KB (242767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7678609a7e25485895fffda9b5eea9f940ffc5e5e34155de64f2933803428c0e`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 5.7 MB (5712861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b6362b379d0e5ed852e577058ae198521bd47c70a6654e5bdd24a5fbc7f326`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79936c5c24a0ca205db9a615d4c0113a2e3093ae64cdabc9a8b1fa930327830c`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca71b03ad3cfece28d778d224d9c61ca3dbea97dc6761af0d411ddb0275f965d`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484f29887b314709fa52867baf4fc140ec7488361c38d1811854c07d682c1451`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9`

```console
$ docker pull nats@sha256:a75b6817e3135f1f789e970a62980e49b9efa3d3cdfc7db4193312f12cb44b3f
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
$ docker pull nats@sha256:cf96338e314ee46e307626e8936dc31b9ef7c67e299b29b7753896d11b52fe8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5455cadbb1bd4919947f5a918491add0f2a8fe5d9aa4a801ca79a4ac8fb308f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:26:10 GMT
COPY file:975a38b1520c81a5e1d0876325548b4aefe0036b6deee1ae7ee20db6abbcc080 in /nats-server 
# Mon, 07 Aug 2023 19:26:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:26:11 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:26:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:26:11 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:26:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc02d5ba29398595681917073dcd141022b8ad8d0da9a18b6f5752e56c86ceea`  
		Last Modified: Mon, 07 Aug 2023 19:26:56 GMT  
		Size: 5.2 MB (5169747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9457cd0af5e7125dfe4a44e1d6d003e2bdaf42da9d1c5f7b313069a145e639`  
		Last Modified: Mon, 07 Aug 2023 19:26:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v6

```console
$ docker pull nats@sha256:3a3792aaaf193e57879f3594e95501c1372bd2a537965db2bc68fd85c13b8cb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4932529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966d4a644152a12918ae66827a94561e477b28d10bd2698612566a5c989612f1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:447be8988a65ae095af689a396d155107ebc910fe545508c6e6af6f1c2d2c4d4 in /nats-server 
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:50:31 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:50:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:50:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:50:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:590d3f4a49d783a9889465cc7862cf43dc4d3a60e0fb075544618efee1ef93e1`  
		Last Modified: Mon, 07 Aug 2023 19:51:13 GMT  
		Size: 4.9 MB (4932022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901e46e20099bb53f1d1b41e9f1cbf04d9af77173e45873723bd9d7825fbbcf0`  
		Last Modified: Mon, 07 Aug 2023 19:51:12 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm variant v7

```console
$ docker pull nats@sha256:3be04f93d99a8e23e99fff2608d9c0d76a4ee2c9c301441f57a2d0b9225c16e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4924573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec722342be0e9d946cb8ac26674a30ff2854116e2e8e1ba75461b3f90d97ecc8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:a28d4beb7d3acaa71be2e58ce3a707a2f5be041842f8a1e4eb4c54dd72e865eb in /nats-server 
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 20:16:33 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 20:16:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 20:16:33 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 20:16:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:68043f4483bff82380b8666c025686881f5483ff754784192f65aa4ec9b662fe`  
		Last Modified: Mon, 07 Aug 2023 20:17:27 GMT  
		Size: 4.9 MB (4924065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0443d8f0ff2c43f481bd49043e2c13423203b3a99754a3baff7df20850bf0e56`  
		Last Modified: Mon, 07 Aug 2023 20:17:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24cb726cdaa647f5307f6d5fa448b299535141c96367b79636f23597407b5071
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4734399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b2f013bc2559b3a905b049fd4b09738b17a4c87d62bed5a1830c6a6e13b1cda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:815b9c4a7d715138f02171cd656c9e8dc6d80e72107c92661c99f6dd24ae2721 in /nats-server 
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:44:14 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:44:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:44:14 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:44:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07116324214b64589e3a471932fe7f6b892068a7cd9cf9bb72a8ea25f8a92200`  
		Last Modified: Mon, 07 Aug 2023 19:44:57 GMT  
		Size: 4.7 MB (4733893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615975e7d25e46607f561d13c4c244d070bb41701a0ac2103df98dcb33e8a4eb`  
		Last Modified: Mon, 07 Aug 2023 19:44:56 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:d8a94368172a3df5204943029b32d7b56dda869dadef4983129598ed86fcec67
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109707647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b1b071e5cf657d3db4c3347053329658550fdb8b09ae38a2618af5b119a8565`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 10 Aug 2023 02:34:53 GMT
RUN cmd /S /C #(nop) COPY file:3b8a3a4f656cc66920d77ff06f41851caa37056073cec32caf7e7024bea62100 in C:\nats-server.exe 
# Thu, 10 Aug 2023 02:34:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 10 Aug 2023 02:34:56 GMT
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
	-	`sha256:6810a6f695e6275423db76be5637667297faaa666b58a9658e1690efe300b007`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 5.2 MB (5242246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fbe96bd125f3ebe2f71079f2d8c4ca1d226d4aa3de1dd2a0fefb0e50421464`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c6c360e7d8fa0f4858a220d96a5d13e7c65c195bb8513191b47c1d3b0c6b91`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3db71fcfd8d9cd70e2947e60d0f27dee2449c365fcd7dde18997017f1f7a443`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112aff03752bdfd32ed33505dc8c488a27bdc249bd506edd30af3d47c0d9b4a2`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine`

```console
$ docker pull nats@sha256:511f5c4cfc6fdd61eb66afab99dfb38bed69aae630d8d5b36bc9bfc716723cd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine` - linux; amd64

```console
$ docker pull nats@sha256:5cf5c3802d1e857d169a3f1d5cbe4799d4839fd6f55af788cedcb6e5a22378e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9195249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4997d3c6db9cae525d31602ba338a453ba4facd93e802fa29b3ba534475bd9f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:26:02 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:26:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:26:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:26:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:26:05 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:26:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:26:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd25bdbc8b4e243f7c3ffdffcc8115824b4b4cb2e9e73e3daadb257d79643d2`  
		Last Modified: Mon, 07 Aug 2023 19:26:33 GMT  
		Size: 5.8 MB (5792639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115edb875772e3386f7d2813cc6497fbdbaea0f7f9a39e552e3309472365aa90`  
		Last Modified: Mon, 07 Aug 2023 19:26:32 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279c31eb6dadb7f2e0ca227988e36fd0206af24465e2a207d488967470b3a63e`  
		Last Modified: Mon, 07 Aug 2023 19:26:32 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:5e07de3c322c8771519734bef7e466ac5028ab54275802d4deb77c36411e3cbb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8700810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e0fee524fb6e7f519b9ae3abd80976c1836c3f10c0be79daf8e035556935b24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:50:24 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:50:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:50:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:50:28 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:50:28 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:50:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:50:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee480b732706005fa701c3c4028a724e52a4fae0fd1c0aa66e0c837002d561d`  
		Last Modified: Mon, 07 Aug 2023 19:50:50 GMT  
		Size: 5.6 MB (5555005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58f30a3786b4a2dc69c83b465d31a4f645160b79da0a61c29860cdc3972b214`  
		Last Modified: Mon, 07 Aug 2023 19:50:49 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e541018b825fe9c407a093e7cac7a09742ba147db4c9b701c8021337ff70ec`  
		Last Modified: Mon, 07 Aug 2023 19:50:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:c4769e1e475367da9b4fc5a660a6fb32b200d27a3d026495fdc5bf74f9388c16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8447620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9893408047cef17e55311c80520a2cceb027a6e9d68f7206dc77b1330526c23e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:16:18 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 20:16:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 20:16:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 20:16:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 20:16:22 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 20:16:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:16:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fca2c62cfb95a8e21097e5398887f17729f82e97f22aba05b4a501ead7235bf`  
		Last Modified: Mon, 07 Aug 2023 20:17:02 GMT  
		Size: 5.5 MB (5547144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c778dd55b3c0df3d1fa0c07a38398ecd9605779c83aad61a071e63327b6077a`  
		Last Modified: Mon, 07 Aug 2023 20:17:00 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f262374e9fca7560e610908419255255f99f7ce00698f5da57b988be8a0827`  
		Last Modified: Mon, 07 Aug 2023 20:17:00 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:280523d3cd269840cf3ca0436eaf836b84057947803f07af5208ef8b7a1f765f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8689649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b733a68b85bf5e9f179e1363356f48edd81ae5fe656cf38413a97a99945327f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:44:08 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:44:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:44:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:44:10 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:44:10 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:44:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:44:10 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7eb0af764262eda43da676eb6212706a1a5c91fc0745feec3c2a78b11feeb74`  
		Last Modified: Mon, 07 Aug 2023 19:44:35 GMT  
		Size: 5.4 MB (5357887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d47d30642d18189ee8bcbc7387c01d1eddb910a0927366bf969f74ba950073`  
		Last Modified: Mon, 07 Aug 2023 19:44:34 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ace711cbe0f8fc6e880cdb92d235a3031e40977634be3a9fe209f05e65a7b7`  
		Last Modified: Mon, 07 Aug 2023 19:44:34 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine3.18`

```console
$ docker pull nats@sha256:511f5c4cfc6fdd61eb66afab99dfb38bed69aae630d8d5b36bc9bfc716723cd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:5cf5c3802d1e857d169a3f1d5cbe4799d4839fd6f55af788cedcb6e5a22378e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9195249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4997d3c6db9cae525d31602ba338a453ba4facd93e802fa29b3ba534475bd9f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:26:02 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:26:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:26:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:26:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:26:05 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:26:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:26:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd25bdbc8b4e243f7c3ffdffcc8115824b4b4cb2e9e73e3daadb257d79643d2`  
		Last Modified: Mon, 07 Aug 2023 19:26:33 GMT  
		Size: 5.8 MB (5792639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115edb875772e3386f7d2813cc6497fbdbaea0f7f9a39e552e3309472365aa90`  
		Last Modified: Mon, 07 Aug 2023 19:26:32 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279c31eb6dadb7f2e0ca227988e36fd0206af24465e2a207d488967470b3a63e`  
		Last Modified: Mon, 07 Aug 2023 19:26:32 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:5e07de3c322c8771519734bef7e466ac5028ab54275802d4deb77c36411e3cbb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8700810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e0fee524fb6e7f519b9ae3abd80976c1836c3f10c0be79daf8e035556935b24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:50:24 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:50:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:50:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:50:28 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:50:28 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:50:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:50:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee480b732706005fa701c3c4028a724e52a4fae0fd1c0aa66e0c837002d561d`  
		Last Modified: Mon, 07 Aug 2023 19:50:50 GMT  
		Size: 5.6 MB (5555005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58f30a3786b4a2dc69c83b465d31a4f645160b79da0a61c29860cdc3972b214`  
		Last Modified: Mon, 07 Aug 2023 19:50:49 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e541018b825fe9c407a093e7cac7a09742ba147db4c9b701c8021337ff70ec`  
		Last Modified: Mon, 07 Aug 2023 19:50:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:c4769e1e475367da9b4fc5a660a6fb32b200d27a3d026495fdc5bf74f9388c16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8447620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9893408047cef17e55311c80520a2cceb027a6e9d68f7206dc77b1330526c23e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:16:18 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 20:16:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 20:16:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 20:16:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 20:16:22 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 20:16:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:16:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fca2c62cfb95a8e21097e5398887f17729f82e97f22aba05b4a501ead7235bf`  
		Last Modified: Mon, 07 Aug 2023 20:17:02 GMT  
		Size: 5.5 MB (5547144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c778dd55b3c0df3d1fa0c07a38398ecd9605779c83aad61a071e63327b6077a`  
		Last Modified: Mon, 07 Aug 2023 20:17:00 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f262374e9fca7560e610908419255255f99f7ce00698f5da57b988be8a0827`  
		Last Modified: Mon, 07 Aug 2023 20:17:00 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:280523d3cd269840cf3ca0436eaf836b84057947803f07af5208ef8b7a1f765f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8689649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b733a68b85bf5e9f179e1363356f48edd81ae5fe656cf38413a97a99945327f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:44:08 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:44:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:44:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:44:10 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:44:10 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:44:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:44:10 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7eb0af764262eda43da676eb6212706a1a5c91fc0745feec3c2a78b11feeb74`  
		Last Modified: Mon, 07 Aug 2023 19:44:35 GMT  
		Size: 5.4 MB (5357887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d47d30642d18189ee8bcbc7387c01d1eddb910a0927366bf969f74ba950073`  
		Last Modified: Mon, 07 Aug 2023 19:44:34 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ace711cbe0f8fc6e880cdb92d235a3031e40977634be3a9fe209f05e65a7b7`  
		Last Modified: Mon, 07 Aug 2023 19:44:34 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-linux`

```console
$ docker pull nats@sha256:3208778cf6c64114c84d0227bfd6fb282f1ba86b85f25c46c410c9e97b3a33ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-linux` - linux; amd64

```console
$ docker pull nats@sha256:cf96338e314ee46e307626e8936dc31b9ef7c67e299b29b7753896d11b52fe8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5455cadbb1bd4919947f5a918491add0f2a8fe5d9aa4a801ca79a4ac8fb308f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:26:10 GMT
COPY file:975a38b1520c81a5e1d0876325548b4aefe0036b6deee1ae7ee20db6abbcc080 in /nats-server 
# Mon, 07 Aug 2023 19:26:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:26:11 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:26:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:26:11 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:26:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc02d5ba29398595681917073dcd141022b8ad8d0da9a18b6f5752e56c86ceea`  
		Last Modified: Mon, 07 Aug 2023 19:26:56 GMT  
		Size: 5.2 MB (5169747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9457cd0af5e7125dfe4a44e1d6d003e2bdaf42da9d1c5f7b313069a145e639`  
		Last Modified: Mon, 07 Aug 2023 19:26:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:3a3792aaaf193e57879f3594e95501c1372bd2a537965db2bc68fd85c13b8cb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4932529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966d4a644152a12918ae66827a94561e477b28d10bd2698612566a5c989612f1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:447be8988a65ae095af689a396d155107ebc910fe545508c6e6af6f1c2d2c4d4 in /nats-server 
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:50:31 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:50:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:50:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:50:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:590d3f4a49d783a9889465cc7862cf43dc4d3a60e0fb075544618efee1ef93e1`  
		Last Modified: Mon, 07 Aug 2023 19:51:13 GMT  
		Size: 4.9 MB (4932022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901e46e20099bb53f1d1b41e9f1cbf04d9af77173e45873723bd9d7825fbbcf0`  
		Last Modified: Mon, 07 Aug 2023 19:51:12 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:3be04f93d99a8e23e99fff2608d9c0d76a4ee2c9c301441f57a2d0b9225c16e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4924573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec722342be0e9d946cb8ac26674a30ff2854116e2e8e1ba75461b3f90d97ecc8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:a28d4beb7d3acaa71be2e58ce3a707a2f5be041842f8a1e4eb4c54dd72e865eb in /nats-server 
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 20:16:33 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 20:16:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 20:16:33 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 20:16:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:68043f4483bff82380b8666c025686881f5483ff754784192f65aa4ec9b662fe`  
		Last Modified: Mon, 07 Aug 2023 20:17:27 GMT  
		Size: 4.9 MB (4924065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0443d8f0ff2c43f481bd49043e2c13423203b3a99754a3baff7df20850bf0e56`  
		Last Modified: Mon, 07 Aug 2023 20:17:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24cb726cdaa647f5307f6d5fa448b299535141c96367b79636f23597407b5071
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4734399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b2f013bc2559b3a905b049fd4b09738b17a4c87d62bed5a1830c6a6e13b1cda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:815b9c4a7d715138f02171cd656c9e8dc6d80e72107c92661c99f6dd24ae2721 in /nats-server 
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:44:14 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:44:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:44:14 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:44:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07116324214b64589e3a471932fe7f6b892068a7cd9cf9bb72a8ea25f8a92200`  
		Last Modified: Mon, 07 Aug 2023 19:44:57 GMT  
		Size: 4.7 MB (4733893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615975e7d25e46607f561d13c4c244d070bb41701a0ac2103df98dcb33e8a4eb`  
		Last Modified: Mon, 07 Aug 2023 19:44:56 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver`

```console
$ docker pull nats@sha256:3959865fd1e3f0b07b7933b6e4772490b619811c09074cfe6fd00985b6614f83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2.9-nanoserver` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:d8a94368172a3df5204943029b32d7b56dda869dadef4983129598ed86fcec67
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109707647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b1b071e5cf657d3db4c3347053329658550fdb8b09ae38a2618af5b119a8565`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 10 Aug 2023 02:34:53 GMT
RUN cmd /S /C #(nop) COPY file:3b8a3a4f656cc66920d77ff06f41851caa37056073cec32caf7e7024bea62100 in C:\nats-server.exe 
# Thu, 10 Aug 2023 02:34:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 10 Aug 2023 02:34:56 GMT
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
	-	`sha256:6810a6f695e6275423db76be5637667297faaa666b58a9658e1690efe300b007`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 5.2 MB (5242246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fbe96bd125f3ebe2f71079f2d8c4ca1d226d4aa3de1dd2a0fefb0e50421464`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c6c360e7d8fa0f4858a220d96a5d13e7c65c195bb8513191b47c1d3b0c6b91`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3db71fcfd8d9cd70e2947e60d0f27dee2449c365fcd7dde18997017f1f7a443`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112aff03752bdfd32ed33505dc8c488a27bdc249bd506edd30af3d47c0d9b4a2`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver-1809`

```console
$ docker pull nats@sha256:3959865fd1e3f0b07b7933b6e4772490b619811c09074cfe6fd00985b6614f83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2.9-nanoserver-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:d8a94368172a3df5204943029b32d7b56dda869dadef4983129598ed86fcec67
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109707647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b1b071e5cf657d3db4c3347053329658550fdb8b09ae38a2618af5b119a8565`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 10 Aug 2023 02:34:53 GMT
RUN cmd /S /C #(nop) COPY file:3b8a3a4f656cc66920d77ff06f41851caa37056073cec32caf7e7024bea62100 in C:\nats-server.exe 
# Thu, 10 Aug 2023 02:34:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 10 Aug 2023 02:34:56 GMT
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
	-	`sha256:6810a6f695e6275423db76be5637667297faaa666b58a9658e1690efe300b007`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 5.2 MB (5242246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fbe96bd125f3ebe2f71079f2d8c4ca1d226d4aa3de1dd2a0fefb0e50421464`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c6c360e7d8fa0f4858a220d96a5d13e7c65c195bb8513191b47c1d3b0c6b91`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3db71fcfd8d9cd70e2947e60d0f27dee2449c365fcd7dde18997017f1f7a443`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112aff03752bdfd32ed33505dc8c488a27bdc249bd506edd30af3d47c0d9b4a2`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-scratch`

```console
$ docker pull nats@sha256:3208778cf6c64114c84d0227bfd6fb282f1ba86b85f25c46c410c9e97b3a33ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-scratch` - linux; amd64

```console
$ docker pull nats@sha256:cf96338e314ee46e307626e8936dc31b9ef7c67e299b29b7753896d11b52fe8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5455cadbb1bd4919947f5a918491add0f2a8fe5d9aa4a801ca79a4ac8fb308f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:26:10 GMT
COPY file:975a38b1520c81a5e1d0876325548b4aefe0036b6deee1ae7ee20db6abbcc080 in /nats-server 
# Mon, 07 Aug 2023 19:26:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:26:11 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:26:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:26:11 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:26:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc02d5ba29398595681917073dcd141022b8ad8d0da9a18b6f5752e56c86ceea`  
		Last Modified: Mon, 07 Aug 2023 19:26:56 GMT  
		Size: 5.2 MB (5169747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9457cd0af5e7125dfe4a44e1d6d003e2bdaf42da9d1c5f7b313069a145e639`  
		Last Modified: Mon, 07 Aug 2023 19:26:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:3a3792aaaf193e57879f3594e95501c1372bd2a537965db2bc68fd85c13b8cb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4932529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966d4a644152a12918ae66827a94561e477b28d10bd2698612566a5c989612f1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:447be8988a65ae095af689a396d155107ebc910fe545508c6e6af6f1c2d2c4d4 in /nats-server 
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:50:31 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:50:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:50:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:50:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:590d3f4a49d783a9889465cc7862cf43dc4d3a60e0fb075544618efee1ef93e1`  
		Last Modified: Mon, 07 Aug 2023 19:51:13 GMT  
		Size: 4.9 MB (4932022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901e46e20099bb53f1d1b41e9f1cbf04d9af77173e45873723bd9d7825fbbcf0`  
		Last Modified: Mon, 07 Aug 2023 19:51:12 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:3be04f93d99a8e23e99fff2608d9c0d76a4ee2c9c301441f57a2d0b9225c16e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4924573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec722342be0e9d946cb8ac26674a30ff2854116e2e8e1ba75461b3f90d97ecc8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:a28d4beb7d3acaa71be2e58ce3a707a2f5be041842f8a1e4eb4c54dd72e865eb in /nats-server 
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 20:16:33 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 20:16:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 20:16:33 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 20:16:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:68043f4483bff82380b8666c025686881f5483ff754784192f65aa4ec9b662fe`  
		Last Modified: Mon, 07 Aug 2023 20:17:27 GMT  
		Size: 4.9 MB (4924065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0443d8f0ff2c43f481bd49043e2c13423203b3a99754a3baff7df20850bf0e56`  
		Last Modified: Mon, 07 Aug 2023 20:17:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24cb726cdaa647f5307f6d5fa448b299535141c96367b79636f23597407b5071
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4734399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b2f013bc2559b3a905b049fd4b09738b17a4c87d62bed5a1830c6a6e13b1cda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:815b9c4a7d715138f02171cd656c9e8dc6d80e72107c92661c99f6dd24ae2721 in /nats-server 
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:44:14 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:44:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:44:14 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:44:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07116324214b64589e3a471932fe7f6b892068a7cd9cf9bb72a8ea25f8a92200`  
		Last Modified: Mon, 07 Aug 2023 19:44:57 GMT  
		Size: 4.7 MB (4733893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615975e7d25e46607f561d13c4c244d070bb41701a0ac2103df98dcb33e8a4eb`  
		Last Modified: Mon, 07 Aug 2023 19:44:56 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore`

```console
$ docker pull nats@sha256:6a5048505a376ddee83a546a4c677bd2c62eaf943530ea64bc946e77b092500c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2.9-windowsservercore` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:df85f652123fd850bc088bf1796ad63e262c83117ef33c913c2324c329e83281
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2001923911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba49e1850a02235e7b24a350ba3483aa40adb3e25011cf8af425be0f74d9bb21`
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
# Thu, 10 Aug 2023 02:32:09 GMT
ENV NATS_SERVER=2.9.21
# Thu, 10 Aug 2023 02:32:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.21/nats-server-v2.9.21-windows-amd64.zip
# Thu, 10 Aug 2023 02:32:11 GMT
ENV NATS_SERVER_SHASUM=43df40bcf81e819e3467a31c548643439d4200486f3032c61ae4b134243f8796
# Thu, 10 Aug 2023 02:33:09 GMT
RUN Set-PSDebug -Trace 2
# Thu, 10 Aug 2023 02:34:42 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 10 Aug 2023 02:34:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 10 Aug 2023 02:34:44 GMT
EXPOSE 4222 6222 8222
# Thu, 10 Aug 2023 02:34:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 10 Aug 2023 02:34:45 GMT
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
	-	`sha256:8065a1cb0e804bbb19260f95fcb2ee724ea73de1da4df8e9744f6498cec33d62`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5638bc45d3356ae277d06dab7b839bf52e16bc50a37408b0de976cebfcd1ab`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc44a5e39ba10538d5f0af74a7c7c00bb731116d9f5f8f19b9469e2464baf901`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98483cb493b32b2587f35850b72b5beb7a5354034943519da2056a8b88a51036`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 242.8 KB (242767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7678609a7e25485895fffda9b5eea9f940ffc5e5e34155de64f2933803428c0e`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 5.7 MB (5712861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b6362b379d0e5ed852e577058ae198521bd47c70a6654e5bdd24a5fbc7f326`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79936c5c24a0ca205db9a615d4c0113a2e3093ae64cdabc9a8b1fa930327830c`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca71b03ad3cfece28d778d224d9c61ca3dbea97dc6761af0d411ddb0275f965d`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484f29887b314709fa52867baf4fc140ec7488361c38d1811854c07d682c1451`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:6a5048505a376ddee83a546a4c677bd2c62eaf943530ea64bc946e77b092500c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2.9-windowsservercore-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:df85f652123fd850bc088bf1796ad63e262c83117ef33c913c2324c329e83281
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2001923911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba49e1850a02235e7b24a350ba3483aa40adb3e25011cf8af425be0f74d9bb21`
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
# Thu, 10 Aug 2023 02:32:09 GMT
ENV NATS_SERVER=2.9.21
# Thu, 10 Aug 2023 02:32:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.21/nats-server-v2.9.21-windows-amd64.zip
# Thu, 10 Aug 2023 02:32:11 GMT
ENV NATS_SERVER_SHASUM=43df40bcf81e819e3467a31c548643439d4200486f3032c61ae4b134243f8796
# Thu, 10 Aug 2023 02:33:09 GMT
RUN Set-PSDebug -Trace 2
# Thu, 10 Aug 2023 02:34:42 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 10 Aug 2023 02:34:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 10 Aug 2023 02:34:44 GMT
EXPOSE 4222 6222 8222
# Thu, 10 Aug 2023 02:34:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 10 Aug 2023 02:34:45 GMT
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
	-	`sha256:8065a1cb0e804bbb19260f95fcb2ee724ea73de1da4df8e9744f6498cec33d62`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5638bc45d3356ae277d06dab7b839bf52e16bc50a37408b0de976cebfcd1ab`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc44a5e39ba10538d5f0af74a7c7c00bb731116d9f5f8f19b9469e2464baf901`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98483cb493b32b2587f35850b72b5beb7a5354034943519da2056a8b88a51036`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 242.8 KB (242767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7678609a7e25485895fffda9b5eea9f940ffc5e5e34155de64f2933803428c0e`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 5.7 MB (5712861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b6362b379d0e5ed852e577058ae198521bd47c70a6654e5bdd24a5fbc7f326`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79936c5c24a0ca205db9a615d4c0113a2e3093ae64cdabc9a8b1fa930327830c`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca71b03ad3cfece28d778d224d9c61ca3dbea97dc6761af0d411ddb0275f965d`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484f29887b314709fa52867baf4fc140ec7488361c38d1811854c07d682c1451`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.21`

```console
$ docker pull nats@sha256:a75b6817e3135f1f789e970a62980e49b9efa3d3cdfc7db4193312f12cb44b3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4737; amd64

### `nats:2.9.21` - linux; amd64

```console
$ docker pull nats@sha256:cf96338e314ee46e307626e8936dc31b9ef7c67e299b29b7753896d11b52fe8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5455cadbb1bd4919947f5a918491add0f2a8fe5d9aa4a801ca79a4ac8fb308f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:26:10 GMT
COPY file:975a38b1520c81a5e1d0876325548b4aefe0036b6deee1ae7ee20db6abbcc080 in /nats-server 
# Mon, 07 Aug 2023 19:26:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:26:11 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:26:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:26:11 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:26:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc02d5ba29398595681917073dcd141022b8ad8d0da9a18b6f5752e56c86ceea`  
		Last Modified: Mon, 07 Aug 2023 19:26:56 GMT  
		Size: 5.2 MB (5169747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9457cd0af5e7125dfe4a44e1d6d003e2bdaf42da9d1c5f7b313069a145e639`  
		Last Modified: Mon, 07 Aug 2023 19:26:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.21` - linux; arm variant v6

```console
$ docker pull nats@sha256:3a3792aaaf193e57879f3594e95501c1372bd2a537965db2bc68fd85c13b8cb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4932529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966d4a644152a12918ae66827a94561e477b28d10bd2698612566a5c989612f1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:447be8988a65ae095af689a396d155107ebc910fe545508c6e6af6f1c2d2c4d4 in /nats-server 
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:50:31 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:50:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:50:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:50:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:590d3f4a49d783a9889465cc7862cf43dc4d3a60e0fb075544618efee1ef93e1`  
		Last Modified: Mon, 07 Aug 2023 19:51:13 GMT  
		Size: 4.9 MB (4932022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901e46e20099bb53f1d1b41e9f1cbf04d9af77173e45873723bd9d7825fbbcf0`  
		Last Modified: Mon, 07 Aug 2023 19:51:12 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.21` - linux; arm variant v7

```console
$ docker pull nats@sha256:3be04f93d99a8e23e99fff2608d9c0d76a4ee2c9c301441f57a2d0b9225c16e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4924573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec722342be0e9d946cb8ac26674a30ff2854116e2e8e1ba75461b3f90d97ecc8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:a28d4beb7d3acaa71be2e58ce3a707a2f5be041842f8a1e4eb4c54dd72e865eb in /nats-server 
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 20:16:33 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 20:16:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 20:16:33 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 20:16:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:68043f4483bff82380b8666c025686881f5483ff754784192f65aa4ec9b662fe`  
		Last Modified: Mon, 07 Aug 2023 20:17:27 GMT  
		Size: 4.9 MB (4924065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0443d8f0ff2c43f481bd49043e2c13423203b3a99754a3baff7df20850bf0e56`  
		Last Modified: Mon, 07 Aug 2023 20:17:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.21` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24cb726cdaa647f5307f6d5fa448b299535141c96367b79636f23597407b5071
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4734399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b2f013bc2559b3a905b049fd4b09738b17a4c87d62bed5a1830c6a6e13b1cda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:815b9c4a7d715138f02171cd656c9e8dc6d80e72107c92661c99f6dd24ae2721 in /nats-server 
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:44:14 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:44:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:44:14 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:44:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07116324214b64589e3a471932fe7f6b892068a7cd9cf9bb72a8ea25f8a92200`  
		Last Modified: Mon, 07 Aug 2023 19:44:57 GMT  
		Size: 4.7 MB (4733893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615975e7d25e46607f561d13c4c244d070bb41701a0ac2103df98dcb33e8a4eb`  
		Last Modified: Mon, 07 Aug 2023 19:44:56 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.21` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:d8a94368172a3df5204943029b32d7b56dda869dadef4983129598ed86fcec67
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109707647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b1b071e5cf657d3db4c3347053329658550fdb8b09ae38a2618af5b119a8565`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 10 Aug 2023 02:34:53 GMT
RUN cmd /S /C #(nop) COPY file:3b8a3a4f656cc66920d77ff06f41851caa37056073cec32caf7e7024bea62100 in C:\nats-server.exe 
# Thu, 10 Aug 2023 02:34:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 10 Aug 2023 02:34:56 GMT
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
	-	`sha256:6810a6f695e6275423db76be5637667297faaa666b58a9658e1690efe300b007`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 5.2 MB (5242246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fbe96bd125f3ebe2f71079f2d8c4ca1d226d4aa3de1dd2a0fefb0e50421464`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c6c360e7d8fa0f4858a220d96a5d13e7c65c195bb8513191b47c1d3b0c6b91`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3db71fcfd8d9cd70e2947e60d0f27dee2449c365fcd7dde18997017f1f7a443`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112aff03752bdfd32ed33505dc8c488a27bdc249bd506edd30af3d47c0d9b4a2`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.21-alpine`

```console
$ docker pull nats@sha256:511f5c4cfc6fdd61eb66afab99dfb38bed69aae630d8d5b36bc9bfc716723cd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.21-alpine` - linux; amd64

```console
$ docker pull nats@sha256:5cf5c3802d1e857d169a3f1d5cbe4799d4839fd6f55af788cedcb6e5a22378e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9195249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4997d3c6db9cae525d31602ba338a453ba4facd93e802fa29b3ba534475bd9f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:26:02 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:26:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:26:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:26:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:26:05 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:26:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:26:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd25bdbc8b4e243f7c3ffdffcc8115824b4b4cb2e9e73e3daadb257d79643d2`  
		Last Modified: Mon, 07 Aug 2023 19:26:33 GMT  
		Size: 5.8 MB (5792639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115edb875772e3386f7d2813cc6497fbdbaea0f7f9a39e552e3309472365aa90`  
		Last Modified: Mon, 07 Aug 2023 19:26:32 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279c31eb6dadb7f2e0ca227988e36fd0206af24465e2a207d488967470b3a63e`  
		Last Modified: Mon, 07 Aug 2023 19:26:32 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.21-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:5e07de3c322c8771519734bef7e466ac5028ab54275802d4deb77c36411e3cbb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8700810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e0fee524fb6e7f519b9ae3abd80976c1836c3f10c0be79daf8e035556935b24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:50:24 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:50:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:50:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:50:28 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:50:28 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:50:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:50:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee480b732706005fa701c3c4028a724e52a4fae0fd1c0aa66e0c837002d561d`  
		Last Modified: Mon, 07 Aug 2023 19:50:50 GMT  
		Size: 5.6 MB (5555005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58f30a3786b4a2dc69c83b465d31a4f645160b79da0a61c29860cdc3972b214`  
		Last Modified: Mon, 07 Aug 2023 19:50:49 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e541018b825fe9c407a093e7cac7a09742ba147db4c9b701c8021337ff70ec`  
		Last Modified: Mon, 07 Aug 2023 19:50:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.21-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:c4769e1e475367da9b4fc5a660a6fb32b200d27a3d026495fdc5bf74f9388c16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8447620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9893408047cef17e55311c80520a2cceb027a6e9d68f7206dc77b1330526c23e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:16:18 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 20:16:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 20:16:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 20:16:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 20:16:22 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 20:16:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:16:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fca2c62cfb95a8e21097e5398887f17729f82e97f22aba05b4a501ead7235bf`  
		Last Modified: Mon, 07 Aug 2023 20:17:02 GMT  
		Size: 5.5 MB (5547144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c778dd55b3c0df3d1fa0c07a38398ecd9605779c83aad61a071e63327b6077a`  
		Last Modified: Mon, 07 Aug 2023 20:17:00 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f262374e9fca7560e610908419255255f99f7ce00698f5da57b988be8a0827`  
		Last Modified: Mon, 07 Aug 2023 20:17:00 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.21-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:280523d3cd269840cf3ca0436eaf836b84057947803f07af5208ef8b7a1f765f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8689649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b733a68b85bf5e9f179e1363356f48edd81ae5fe656cf38413a97a99945327f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:44:08 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:44:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:44:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:44:10 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:44:10 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:44:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:44:10 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7eb0af764262eda43da676eb6212706a1a5c91fc0745feec3c2a78b11feeb74`  
		Last Modified: Mon, 07 Aug 2023 19:44:35 GMT  
		Size: 5.4 MB (5357887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d47d30642d18189ee8bcbc7387c01d1eddb910a0927366bf969f74ba950073`  
		Last Modified: Mon, 07 Aug 2023 19:44:34 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ace711cbe0f8fc6e880cdb92d235a3031e40977634be3a9fe209f05e65a7b7`  
		Last Modified: Mon, 07 Aug 2023 19:44:34 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.21-alpine3.18`

```console
$ docker pull nats@sha256:511f5c4cfc6fdd61eb66afab99dfb38bed69aae630d8d5b36bc9bfc716723cd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.21-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:5cf5c3802d1e857d169a3f1d5cbe4799d4839fd6f55af788cedcb6e5a22378e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9195249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4997d3c6db9cae525d31602ba338a453ba4facd93e802fa29b3ba534475bd9f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:26:02 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:26:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:26:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:26:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:26:05 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:26:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:26:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd25bdbc8b4e243f7c3ffdffcc8115824b4b4cb2e9e73e3daadb257d79643d2`  
		Last Modified: Mon, 07 Aug 2023 19:26:33 GMT  
		Size: 5.8 MB (5792639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115edb875772e3386f7d2813cc6497fbdbaea0f7f9a39e552e3309472365aa90`  
		Last Modified: Mon, 07 Aug 2023 19:26:32 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279c31eb6dadb7f2e0ca227988e36fd0206af24465e2a207d488967470b3a63e`  
		Last Modified: Mon, 07 Aug 2023 19:26:32 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.21-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:5e07de3c322c8771519734bef7e466ac5028ab54275802d4deb77c36411e3cbb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8700810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e0fee524fb6e7f519b9ae3abd80976c1836c3f10c0be79daf8e035556935b24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:50:24 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:50:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:50:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:50:28 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:50:28 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:50:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:50:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee480b732706005fa701c3c4028a724e52a4fae0fd1c0aa66e0c837002d561d`  
		Last Modified: Mon, 07 Aug 2023 19:50:50 GMT  
		Size: 5.6 MB (5555005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58f30a3786b4a2dc69c83b465d31a4f645160b79da0a61c29860cdc3972b214`  
		Last Modified: Mon, 07 Aug 2023 19:50:49 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e541018b825fe9c407a093e7cac7a09742ba147db4c9b701c8021337ff70ec`  
		Last Modified: Mon, 07 Aug 2023 19:50:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.21-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:c4769e1e475367da9b4fc5a660a6fb32b200d27a3d026495fdc5bf74f9388c16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8447620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9893408047cef17e55311c80520a2cceb027a6e9d68f7206dc77b1330526c23e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:16:18 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 20:16:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 20:16:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 20:16:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 20:16:22 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 20:16:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:16:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fca2c62cfb95a8e21097e5398887f17729f82e97f22aba05b4a501ead7235bf`  
		Last Modified: Mon, 07 Aug 2023 20:17:02 GMT  
		Size: 5.5 MB (5547144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c778dd55b3c0df3d1fa0c07a38398ecd9605779c83aad61a071e63327b6077a`  
		Last Modified: Mon, 07 Aug 2023 20:17:00 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f262374e9fca7560e610908419255255f99f7ce00698f5da57b988be8a0827`  
		Last Modified: Mon, 07 Aug 2023 20:17:00 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.21-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:280523d3cd269840cf3ca0436eaf836b84057947803f07af5208ef8b7a1f765f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8689649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b733a68b85bf5e9f179e1363356f48edd81ae5fe656cf38413a97a99945327f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:44:08 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:44:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:44:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:44:10 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:44:10 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:44:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:44:10 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7eb0af764262eda43da676eb6212706a1a5c91fc0745feec3c2a78b11feeb74`  
		Last Modified: Mon, 07 Aug 2023 19:44:35 GMT  
		Size: 5.4 MB (5357887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d47d30642d18189ee8bcbc7387c01d1eddb910a0927366bf969f74ba950073`  
		Last Modified: Mon, 07 Aug 2023 19:44:34 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ace711cbe0f8fc6e880cdb92d235a3031e40977634be3a9fe209f05e65a7b7`  
		Last Modified: Mon, 07 Aug 2023 19:44:34 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.21-linux`

```console
$ docker pull nats@sha256:3208778cf6c64114c84d0227bfd6fb282f1ba86b85f25c46c410c9e97b3a33ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.21-linux` - linux; amd64

```console
$ docker pull nats@sha256:cf96338e314ee46e307626e8936dc31b9ef7c67e299b29b7753896d11b52fe8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5455cadbb1bd4919947f5a918491add0f2a8fe5d9aa4a801ca79a4ac8fb308f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:26:10 GMT
COPY file:975a38b1520c81a5e1d0876325548b4aefe0036b6deee1ae7ee20db6abbcc080 in /nats-server 
# Mon, 07 Aug 2023 19:26:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:26:11 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:26:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:26:11 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:26:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc02d5ba29398595681917073dcd141022b8ad8d0da9a18b6f5752e56c86ceea`  
		Last Modified: Mon, 07 Aug 2023 19:26:56 GMT  
		Size: 5.2 MB (5169747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9457cd0af5e7125dfe4a44e1d6d003e2bdaf42da9d1c5f7b313069a145e639`  
		Last Modified: Mon, 07 Aug 2023 19:26:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.21-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:3a3792aaaf193e57879f3594e95501c1372bd2a537965db2bc68fd85c13b8cb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4932529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966d4a644152a12918ae66827a94561e477b28d10bd2698612566a5c989612f1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:447be8988a65ae095af689a396d155107ebc910fe545508c6e6af6f1c2d2c4d4 in /nats-server 
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:50:31 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:50:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:50:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:50:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:590d3f4a49d783a9889465cc7862cf43dc4d3a60e0fb075544618efee1ef93e1`  
		Last Modified: Mon, 07 Aug 2023 19:51:13 GMT  
		Size: 4.9 MB (4932022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901e46e20099bb53f1d1b41e9f1cbf04d9af77173e45873723bd9d7825fbbcf0`  
		Last Modified: Mon, 07 Aug 2023 19:51:12 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.21-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:3be04f93d99a8e23e99fff2608d9c0d76a4ee2c9c301441f57a2d0b9225c16e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4924573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec722342be0e9d946cb8ac26674a30ff2854116e2e8e1ba75461b3f90d97ecc8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:a28d4beb7d3acaa71be2e58ce3a707a2f5be041842f8a1e4eb4c54dd72e865eb in /nats-server 
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 20:16:33 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 20:16:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 20:16:33 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 20:16:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:68043f4483bff82380b8666c025686881f5483ff754784192f65aa4ec9b662fe`  
		Last Modified: Mon, 07 Aug 2023 20:17:27 GMT  
		Size: 4.9 MB (4924065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0443d8f0ff2c43f481bd49043e2c13423203b3a99754a3baff7df20850bf0e56`  
		Last Modified: Mon, 07 Aug 2023 20:17:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.21-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24cb726cdaa647f5307f6d5fa448b299535141c96367b79636f23597407b5071
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4734399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b2f013bc2559b3a905b049fd4b09738b17a4c87d62bed5a1830c6a6e13b1cda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:815b9c4a7d715138f02171cd656c9e8dc6d80e72107c92661c99f6dd24ae2721 in /nats-server 
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:44:14 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:44:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:44:14 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:44:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07116324214b64589e3a471932fe7f6b892068a7cd9cf9bb72a8ea25f8a92200`  
		Last Modified: Mon, 07 Aug 2023 19:44:57 GMT  
		Size: 4.7 MB (4733893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615975e7d25e46607f561d13c4c244d070bb41701a0ac2103df98dcb33e8a4eb`  
		Last Modified: Mon, 07 Aug 2023 19:44:56 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.21-nanoserver`

```console
$ docker pull nats@sha256:3959865fd1e3f0b07b7933b6e4772490b619811c09074cfe6fd00985b6614f83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2.9.21-nanoserver` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:d8a94368172a3df5204943029b32d7b56dda869dadef4983129598ed86fcec67
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109707647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b1b071e5cf657d3db4c3347053329658550fdb8b09ae38a2618af5b119a8565`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 10 Aug 2023 02:34:53 GMT
RUN cmd /S /C #(nop) COPY file:3b8a3a4f656cc66920d77ff06f41851caa37056073cec32caf7e7024bea62100 in C:\nats-server.exe 
# Thu, 10 Aug 2023 02:34:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 10 Aug 2023 02:34:56 GMT
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
	-	`sha256:6810a6f695e6275423db76be5637667297faaa666b58a9658e1690efe300b007`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 5.2 MB (5242246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fbe96bd125f3ebe2f71079f2d8c4ca1d226d4aa3de1dd2a0fefb0e50421464`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c6c360e7d8fa0f4858a220d96a5d13e7c65c195bb8513191b47c1d3b0c6b91`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3db71fcfd8d9cd70e2947e60d0f27dee2449c365fcd7dde18997017f1f7a443`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112aff03752bdfd32ed33505dc8c488a27bdc249bd506edd30af3d47c0d9b4a2`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.21-nanoserver-1809`

```console
$ docker pull nats@sha256:3959865fd1e3f0b07b7933b6e4772490b619811c09074cfe6fd00985b6614f83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2.9.21-nanoserver-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:d8a94368172a3df5204943029b32d7b56dda869dadef4983129598ed86fcec67
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109707647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b1b071e5cf657d3db4c3347053329658550fdb8b09ae38a2618af5b119a8565`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 10 Aug 2023 02:34:53 GMT
RUN cmd /S /C #(nop) COPY file:3b8a3a4f656cc66920d77ff06f41851caa37056073cec32caf7e7024bea62100 in C:\nats-server.exe 
# Thu, 10 Aug 2023 02:34:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 10 Aug 2023 02:34:56 GMT
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
	-	`sha256:6810a6f695e6275423db76be5637667297faaa666b58a9658e1690efe300b007`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 5.2 MB (5242246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fbe96bd125f3ebe2f71079f2d8c4ca1d226d4aa3de1dd2a0fefb0e50421464`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c6c360e7d8fa0f4858a220d96a5d13e7c65c195bb8513191b47c1d3b0c6b91`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3db71fcfd8d9cd70e2947e60d0f27dee2449c365fcd7dde18997017f1f7a443`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112aff03752bdfd32ed33505dc8c488a27bdc249bd506edd30af3d47c0d9b4a2`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.21-scratch`

```console
$ docker pull nats@sha256:3208778cf6c64114c84d0227bfd6fb282f1ba86b85f25c46c410c9e97b3a33ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.21-scratch` - linux; amd64

```console
$ docker pull nats@sha256:cf96338e314ee46e307626e8936dc31b9ef7c67e299b29b7753896d11b52fe8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5455cadbb1bd4919947f5a918491add0f2a8fe5d9aa4a801ca79a4ac8fb308f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:26:10 GMT
COPY file:975a38b1520c81a5e1d0876325548b4aefe0036b6deee1ae7ee20db6abbcc080 in /nats-server 
# Mon, 07 Aug 2023 19:26:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:26:11 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:26:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:26:11 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:26:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc02d5ba29398595681917073dcd141022b8ad8d0da9a18b6f5752e56c86ceea`  
		Last Modified: Mon, 07 Aug 2023 19:26:56 GMT  
		Size: 5.2 MB (5169747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9457cd0af5e7125dfe4a44e1d6d003e2bdaf42da9d1c5f7b313069a145e639`  
		Last Modified: Mon, 07 Aug 2023 19:26:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.21-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:3a3792aaaf193e57879f3594e95501c1372bd2a537965db2bc68fd85c13b8cb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4932529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966d4a644152a12918ae66827a94561e477b28d10bd2698612566a5c989612f1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:447be8988a65ae095af689a396d155107ebc910fe545508c6e6af6f1c2d2c4d4 in /nats-server 
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:50:31 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:50:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:50:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:50:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:590d3f4a49d783a9889465cc7862cf43dc4d3a60e0fb075544618efee1ef93e1`  
		Last Modified: Mon, 07 Aug 2023 19:51:13 GMT  
		Size: 4.9 MB (4932022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901e46e20099bb53f1d1b41e9f1cbf04d9af77173e45873723bd9d7825fbbcf0`  
		Last Modified: Mon, 07 Aug 2023 19:51:12 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.21-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:3be04f93d99a8e23e99fff2608d9c0d76a4ee2c9c301441f57a2d0b9225c16e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4924573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec722342be0e9d946cb8ac26674a30ff2854116e2e8e1ba75461b3f90d97ecc8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:a28d4beb7d3acaa71be2e58ce3a707a2f5be041842f8a1e4eb4c54dd72e865eb in /nats-server 
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 20:16:33 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 20:16:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 20:16:33 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 20:16:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:68043f4483bff82380b8666c025686881f5483ff754784192f65aa4ec9b662fe`  
		Last Modified: Mon, 07 Aug 2023 20:17:27 GMT  
		Size: 4.9 MB (4924065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0443d8f0ff2c43f481bd49043e2c13423203b3a99754a3baff7df20850bf0e56`  
		Last Modified: Mon, 07 Aug 2023 20:17:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.21-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24cb726cdaa647f5307f6d5fa448b299535141c96367b79636f23597407b5071
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4734399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b2f013bc2559b3a905b049fd4b09738b17a4c87d62bed5a1830c6a6e13b1cda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:815b9c4a7d715138f02171cd656c9e8dc6d80e72107c92661c99f6dd24ae2721 in /nats-server 
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:44:14 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:44:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:44:14 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:44:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07116324214b64589e3a471932fe7f6b892068a7cd9cf9bb72a8ea25f8a92200`  
		Last Modified: Mon, 07 Aug 2023 19:44:57 GMT  
		Size: 4.7 MB (4733893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615975e7d25e46607f561d13c4c244d070bb41701a0ac2103df98dcb33e8a4eb`  
		Last Modified: Mon, 07 Aug 2023 19:44:56 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.21-windowsservercore`

```console
$ docker pull nats@sha256:6a5048505a376ddee83a546a4c677bd2c62eaf943530ea64bc946e77b092500c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2.9.21-windowsservercore` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:df85f652123fd850bc088bf1796ad63e262c83117ef33c913c2324c329e83281
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2001923911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba49e1850a02235e7b24a350ba3483aa40adb3e25011cf8af425be0f74d9bb21`
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
# Thu, 10 Aug 2023 02:32:09 GMT
ENV NATS_SERVER=2.9.21
# Thu, 10 Aug 2023 02:32:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.21/nats-server-v2.9.21-windows-amd64.zip
# Thu, 10 Aug 2023 02:32:11 GMT
ENV NATS_SERVER_SHASUM=43df40bcf81e819e3467a31c548643439d4200486f3032c61ae4b134243f8796
# Thu, 10 Aug 2023 02:33:09 GMT
RUN Set-PSDebug -Trace 2
# Thu, 10 Aug 2023 02:34:42 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 10 Aug 2023 02:34:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 10 Aug 2023 02:34:44 GMT
EXPOSE 4222 6222 8222
# Thu, 10 Aug 2023 02:34:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 10 Aug 2023 02:34:45 GMT
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
	-	`sha256:8065a1cb0e804bbb19260f95fcb2ee724ea73de1da4df8e9744f6498cec33d62`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5638bc45d3356ae277d06dab7b839bf52e16bc50a37408b0de976cebfcd1ab`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc44a5e39ba10538d5f0af74a7c7c00bb731116d9f5f8f19b9469e2464baf901`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98483cb493b32b2587f35850b72b5beb7a5354034943519da2056a8b88a51036`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 242.8 KB (242767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7678609a7e25485895fffda9b5eea9f940ffc5e5e34155de64f2933803428c0e`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 5.7 MB (5712861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b6362b379d0e5ed852e577058ae198521bd47c70a6654e5bdd24a5fbc7f326`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79936c5c24a0ca205db9a615d4c0113a2e3093ae64cdabc9a8b1fa930327830c`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca71b03ad3cfece28d778d224d9c61ca3dbea97dc6761af0d411ddb0275f965d`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484f29887b314709fa52867baf4fc140ec7488361c38d1811854c07d682c1451`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.21-windowsservercore-1809`

```console
$ docker pull nats@sha256:6a5048505a376ddee83a546a4c677bd2c62eaf943530ea64bc946e77b092500c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:2.9.21-windowsservercore-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:df85f652123fd850bc088bf1796ad63e262c83117ef33c913c2324c329e83281
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2001923911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba49e1850a02235e7b24a350ba3483aa40adb3e25011cf8af425be0f74d9bb21`
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
# Thu, 10 Aug 2023 02:32:09 GMT
ENV NATS_SERVER=2.9.21
# Thu, 10 Aug 2023 02:32:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.21/nats-server-v2.9.21-windows-amd64.zip
# Thu, 10 Aug 2023 02:32:11 GMT
ENV NATS_SERVER_SHASUM=43df40bcf81e819e3467a31c548643439d4200486f3032c61ae4b134243f8796
# Thu, 10 Aug 2023 02:33:09 GMT
RUN Set-PSDebug -Trace 2
# Thu, 10 Aug 2023 02:34:42 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 10 Aug 2023 02:34:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 10 Aug 2023 02:34:44 GMT
EXPOSE 4222 6222 8222
# Thu, 10 Aug 2023 02:34:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 10 Aug 2023 02:34:45 GMT
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
	-	`sha256:8065a1cb0e804bbb19260f95fcb2ee724ea73de1da4df8e9744f6498cec33d62`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5638bc45d3356ae277d06dab7b839bf52e16bc50a37408b0de976cebfcd1ab`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc44a5e39ba10538d5f0af74a7c7c00bb731116d9f5f8f19b9469e2464baf901`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98483cb493b32b2587f35850b72b5beb7a5354034943519da2056a8b88a51036`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 242.8 KB (242767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7678609a7e25485895fffda9b5eea9f940ffc5e5e34155de64f2933803428c0e`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 5.7 MB (5712861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b6362b379d0e5ed852e577058ae198521bd47c70a6654e5bdd24a5fbc7f326`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79936c5c24a0ca205db9a615d4c0113a2e3093ae64cdabc9a8b1fa930327830c`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca71b03ad3cfece28d778d224d9c61ca3dbea97dc6761af0d411ddb0275f965d`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484f29887b314709fa52867baf4fc140ec7488361c38d1811854c07d682c1451`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:511f5c4cfc6fdd61eb66afab99dfb38bed69aae630d8d5b36bc9bfc716723cd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:5cf5c3802d1e857d169a3f1d5cbe4799d4839fd6f55af788cedcb6e5a22378e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9195249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4997d3c6db9cae525d31602ba338a453ba4facd93e802fa29b3ba534475bd9f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:26:02 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:26:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:26:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:26:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:26:05 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:26:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:26:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd25bdbc8b4e243f7c3ffdffcc8115824b4b4cb2e9e73e3daadb257d79643d2`  
		Last Modified: Mon, 07 Aug 2023 19:26:33 GMT  
		Size: 5.8 MB (5792639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115edb875772e3386f7d2813cc6497fbdbaea0f7f9a39e552e3309472365aa90`  
		Last Modified: Mon, 07 Aug 2023 19:26:32 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279c31eb6dadb7f2e0ca227988e36fd0206af24465e2a207d488967470b3a63e`  
		Last Modified: Mon, 07 Aug 2023 19:26:32 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:5e07de3c322c8771519734bef7e466ac5028ab54275802d4deb77c36411e3cbb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8700810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e0fee524fb6e7f519b9ae3abd80976c1836c3f10c0be79daf8e035556935b24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:50:24 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:50:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:50:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:50:28 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:50:28 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:50:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:50:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee480b732706005fa701c3c4028a724e52a4fae0fd1c0aa66e0c837002d561d`  
		Last Modified: Mon, 07 Aug 2023 19:50:50 GMT  
		Size: 5.6 MB (5555005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58f30a3786b4a2dc69c83b465d31a4f645160b79da0a61c29860cdc3972b214`  
		Last Modified: Mon, 07 Aug 2023 19:50:49 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e541018b825fe9c407a093e7cac7a09742ba147db4c9b701c8021337ff70ec`  
		Last Modified: Mon, 07 Aug 2023 19:50:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:c4769e1e475367da9b4fc5a660a6fb32b200d27a3d026495fdc5bf74f9388c16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8447620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9893408047cef17e55311c80520a2cceb027a6e9d68f7206dc77b1330526c23e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:16:18 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 20:16:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 20:16:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 20:16:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 20:16:22 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 20:16:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:16:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fca2c62cfb95a8e21097e5398887f17729f82e97f22aba05b4a501ead7235bf`  
		Last Modified: Mon, 07 Aug 2023 20:17:02 GMT  
		Size: 5.5 MB (5547144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c778dd55b3c0df3d1fa0c07a38398ecd9605779c83aad61a071e63327b6077a`  
		Last Modified: Mon, 07 Aug 2023 20:17:00 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f262374e9fca7560e610908419255255f99f7ce00698f5da57b988be8a0827`  
		Last Modified: Mon, 07 Aug 2023 20:17:00 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:280523d3cd269840cf3ca0436eaf836b84057947803f07af5208ef8b7a1f765f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8689649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b733a68b85bf5e9f179e1363356f48edd81ae5fe656cf38413a97a99945327f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:44:08 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:44:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:44:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:44:10 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:44:10 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:44:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:44:10 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7eb0af764262eda43da676eb6212706a1a5c91fc0745feec3c2a78b11feeb74`  
		Last Modified: Mon, 07 Aug 2023 19:44:35 GMT  
		Size: 5.4 MB (5357887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d47d30642d18189ee8bcbc7387c01d1eddb910a0927366bf969f74ba950073`  
		Last Modified: Mon, 07 Aug 2023 19:44:34 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ace711cbe0f8fc6e880cdb92d235a3031e40977634be3a9fe209f05e65a7b7`  
		Last Modified: Mon, 07 Aug 2023 19:44:34 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.18`

```console
$ docker pull nats@sha256:511f5c4cfc6fdd61eb66afab99dfb38bed69aae630d8d5b36bc9bfc716723cd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:5cf5c3802d1e857d169a3f1d5cbe4799d4839fd6f55af788cedcb6e5a22378e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.2 MB (9195249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4997d3c6db9cae525d31602ba338a453ba4facd93e802fa29b3ba534475bd9f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:26:02 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:26:05 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:26:05 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:26:05 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:26:05 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:26:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:26:05 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd25bdbc8b4e243f7c3ffdffcc8115824b4b4cb2e9e73e3daadb257d79643d2`  
		Last Modified: Mon, 07 Aug 2023 19:26:33 GMT  
		Size: 5.8 MB (5792639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:115edb875772e3386f7d2813cc6497fbdbaea0f7f9a39e552e3309472365aa90`  
		Last Modified: Mon, 07 Aug 2023 19:26:32 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279c31eb6dadb7f2e0ca227988e36fd0206af24465e2a207d488967470b3a63e`  
		Last Modified: Mon, 07 Aug 2023 19:26:32 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:5e07de3c322c8771519734bef7e466ac5028ab54275802d4deb77c36411e3cbb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8700810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e0fee524fb6e7f519b9ae3abd80976c1836c3f10c0be79daf8e035556935b24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:14 GMT
ADD file:9882e99e5f94ab2db05c029648ac5be7cf0f063a8701394fcbb543a7ef5d4b90 in / 
# Mon, 07 Aug 2023 19:49:15 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:50:24 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:50:27 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:50:27 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:50:28 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:50:28 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:50:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:50:28 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:af09961d4a43b504efc76e38b50918977c28be73eeb8b926247783a00e8b9f2f`  
		Last Modified: Mon, 07 Aug 2023 19:49:38 GMT  
		Size: 3.1 MB (3144809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee480b732706005fa701c3c4028a724e52a4fae0fd1c0aa66e0c837002d561d`  
		Last Modified: Mon, 07 Aug 2023 19:50:50 GMT  
		Size: 5.6 MB (5555005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58f30a3786b4a2dc69c83b465d31a4f645160b79da0a61c29860cdc3972b214`  
		Last Modified: Mon, 07 Aug 2023 19:50:49 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e541018b825fe9c407a093e7cac7a09742ba147db4c9b701c8021337ff70ec`  
		Last Modified: Mon, 07 Aug 2023 19:50:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:c4769e1e475367da9b4fc5a660a6fb32b200d27a3d026495fdc5bf74f9388c16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.4 MB (8447620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9893408047cef17e55311c80520a2cceb027a6e9d68f7206dc77b1330526c23e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:25 GMT
ADD file:e3f56488d3d3bb67729714db13ddadf6652e7efb5281cfc7010d3e71f9d6607f in / 
# Mon, 07 Aug 2023 19:57:25 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:16:18 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 20:16:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 20:16:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 20:16:22 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 20:16:22 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 20:16:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 20:16:23 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:f8dec92eec42224ef9e6ca9c6207ea6b9195dcf93d06bd5ceff0f814b62bf064`  
		Last Modified: Mon, 07 Aug 2023 19:57:55 GMT  
		Size: 2.9 MB (2899480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fca2c62cfb95a8e21097e5398887f17729f82e97f22aba05b4a501ead7235bf`  
		Last Modified: Mon, 07 Aug 2023 20:17:02 GMT  
		Size: 5.5 MB (5547144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c778dd55b3c0df3d1fa0c07a38398ecd9605779c83aad61a071e63327b6077a`  
		Last Modified: Mon, 07 Aug 2023 20:17:00 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f262374e9fca7560e610908419255255f99f7ce00698f5da57b988be8a0827`  
		Last Modified: Mon, 07 Aug 2023 20:17:00 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:280523d3cd269840cf3ca0436eaf836b84057947803f07af5208ef8b7a1f765f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8689649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b733a68b85bf5e9f179e1363356f48edd81ae5fe656cf38413a97a99945327f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 19:44:08 GMT
ENV NATS_SERVER=2.9.21
# Mon, 07 Aug 2023 19:44:10 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='6c2906b5a3b930e842c0a88772b5f484e962ac342f57852a45b1c5a7e10f2197' ;; 		armhf) natsArch='arm6'; sha256='424576d72c1f3b5bd309254d0d0462e21b4aaf6b85defcf6663128294b15c16f' ;; 		armv7) natsArch='arm7'; sha256='3ee6e4db568311c6832b1ec4d76933cc8ee1a783281ed89da5ebe6f602d1c521' ;; 		x86_64) natsArch='amd64'; sha256='2bd2878a63efa5bc9b9c3f1d43fd953c7e14b22ba540f7dea19f7fb3a803215d' ;; 		x86) natsArch='386'; sha256='6eef61e4a81fb03f47ef8bfe08eab6909846a3404db28b4260630385dc27910f' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 07 Aug 2023 19:44:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 07 Aug 2023 19:44:10 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 07 Aug 2023 19:44:10 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:44:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 07 Aug 2023 19:44:10 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7eb0af764262eda43da676eb6212706a1a5c91fc0745feec3c2a78b11feeb74`  
		Last Modified: Mon, 07 Aug 2023 19:44:35 GMT  
		Size: 5.4 MB (5357887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d47d30642d18189ee8bcbc7387c01d1eddb910a0927366bf969f74ba950073`  
		Last Modified: Mon, 07 Aug 2023 19:44:34 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ace711cbe0f8fc6e880cdb92d235a3031e40977634be3a9fe209f05e65a7b7`  
		Last Modified: Mon, 07 Aug 2023 19:44:34 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:a75b6817e3135f1f789e970a62980e49b9efa3d3cdfc7db4193312f12cb44b3f
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
$ docker pull nats@sha256:cf96338e314ee46e307626e8936dc31b9ef7c67e299b29b7753896d11b52fe8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5455cadbb1bd4919947f5a918491add0f2a8fe5d9aa4a801ca79a4ac8fb308f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:26:10 GMT
COPY file:975a38b1520c81a5e1d0876325548b4aefe0036b6deee1ae7ee20db6abbcc080 in /nats-server 
# Mon, 07 Aug 2023 19:26:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:26:11 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:26:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:26:11 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:26:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc02d5ba29398595681917073dcd141022b8ad8d0da9a18b6f5752e56c86ceea`  
		Last Modified: Mon, 07 Aug 2023 19:26:56 GMT  
		Size: 5.2 MB (5169747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9457cd0af5e7125dfe4a44e1d6d003e2bdaf42da9d1c5f7b313069a145e639`  
		Last Modified: Mon, 07 Aug 2023 19:26:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:3a3792aaaf193e57879f3594e95501c1372bd2a537965db2bc68fd85c13b8cb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4932529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966d4a644152a12918ae66827a94561e477b28d10bd2698612566a5c989612f1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:447be8988a65ae095af689a396d155107ebc910fe545508c6e6af6f1c2d2c4d4 in /nats-server 
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:50:31 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:50:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:50:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:50:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:590d3f4a49d783a9889465cc7862cf43dc4d3a60e0fb075544618efee1ef93e1`  
		Last Modified: Mon, 07 Aug 2023 19:51:13 GMT  
		Size: 4.9 MB (4932022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901e46e20099bb53f1d1b41e9f1cbf04d9af77173e45873723bd9d7825fbbcf0`  
		Last Modified: Mon, 07 Aug 2023 19:51:12 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:3be04f93d99a8e23e99fff2608d9c0d76a4ee2c9c301441f57a2d0b9225c16e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4924573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec722342be0e9d946cb8ac26674a30ff2854116e2e8e1ba75461b3f90d97ecc8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:a28d4beb7d3acaa71be2e58ce3a707a2f5be041842f8a1e4eb4c54dd72e865eb in /nats-server 
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 20:16:33 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 20:16:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 20:16:33 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 20:16:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:68043f4483bff82380b8666c025686881f5483ff754784192f65aa4ec9b662fe`  
		Last Modified: Mon, 07 Aug 2023 20:17:27 GMT  
		Size: 4.9 MB (4924065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0443d8f0ff2c43f481bd49043e2c13423203b3a99754a3baff7df20850bf0e56`  
		Last Modified: Mon, 07 Aug 2023 20:17:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24cb726cdaa647f5307f6d5fa448b299535141c96367b79636f23597407b5071
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4734399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b2f013bc2559b3a905b049fd4b09738b17a4c87d62bed5a1830c6a6e13b1cda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:815b9c4a7d715138f02171cd656c9e8dc6d80e72107c92661c99f6dd24ae2721 in /nats-server 
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:44:14 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:44:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:44:14 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:44:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07116324214b64589e3a471932fe7f6b892068a7cd9cf9bb72a8ea25f8a92200`  
		Last Modified: Mon, 07 Aug 2023 19:44:57 GMT  
		Size: 4.7 MB (4733893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615975e7d25e46607f561d13c4c244d070bb41701a0ac2103df98dcb33e8a4eb`  
		Last Modified: Mon, 07 Aug 2023 19:44:56 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:d8a94368172a3df5204943029b32d7b56dda869dadef4983129598ed86fcec67
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109707647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b1b071e5cf657d3db4c3347053329658550fdb8b09ae38a2618af5b119a8565`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 10 Aug 2023 02:34:53 GMT
RUN cmd /S /C #(nop) COPY file:3b8a3a4f656cc66920d77ff06f41851caa37056073cec32caf7e7024bea62100 in C:\nats-server.exe 
# Thu, 10 Aug 2023 02:34:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 10 Aug 2023 02:34:56 GMT
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
	-	`sha256:6810a6f695e6275423db76be5637667297faaa666b58a9658e1690efe300b007`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 5.2 MB (5242246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fbe96bd125f3ebe2f71079f2d8c4ca1d226d4aa3de1dd2a0fefb0e50421464`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c6c360e7d8fa0f4858a220d96a5d13e7c65c195bb8513191b47c1d3b0c6b91`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3db71fcfd8d9cd70e2947e60d0f27dee2449c365fcd7dde18997017f1f7a443`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112aff03752bdfd32ed33505dc8c488a27bdc249bd506edd30af3d47c0d9b4a2`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:3208778cf6c64114c84d0227bfd6fb282f1ba86b85f25c46c410c9e97b3a33ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:cf96338e314ee46e307626e8936dc31b9ef7c67e299b29b7753896d11b52fe8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5455cadbb1bd4919947f5a918491add0f2a8fe5d9aa4a801ca79a4ac8fb308f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:26:10 GMT
COPY file:975a38b1520c81a5e1d0876325548b4aefe0036b6deee1ae7ee20db6abbcc080 in /nats-server 
# Mon, 07 Aug 2023 19:26:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:26:11 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:26:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:26:11 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:26:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc02d5ba29398595681917073dcd141022b8ad8d0da9a18b6f5752e56c86ceea`  
		Last Modified: Mon, 07 Aug 2023 19:26:56 GMT  
		Size: 5.2 MB (5169747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9457cd0af5e7125dfe4a44e1d6d003e2bdaf42da9d1c5f7b313069a145e639`  
		Last Modified: Mon, 07 Aug 2023 19:26:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:3a3792aaaf193e57879f3594e95501c1372bd2a537965db2bc68fd85c13b8cb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4932529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966d4a644152a12918ae66827a94561e477b28d10bd2698612566a5c989612f1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:447be8988a65ae095af689a396d155107ebc910fe545508c6e6af6f1c2d2c4d4 in /nats-server 
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:50:31 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:50:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:50:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:50:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:590d3f4a49d783a9889465cc7862cf43dc4d3a60e0fb075544618efee1ef93e1`  
		Last Modified: Mon, 07 Aug 2023 19:51:13 GMT  
		Size: 4.9 MB (4932022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901e46e20099bb53f1d1b41e9f1cbf04d9af77173e45873723bd9d7825fbbcf0`  
		Last Modified: Mon, 07 Aug 2023 19:51:12 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:3be04f93d99a8e23e99fff2608d9c0d76a4ee2c9c301441f57a2d0b9225c16e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4924573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec722342be0e9d946cb8ac26674a30ff2854116e2e8e1ba75461b3f90d97ecc8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:a28d4beb7d3acaa71be2e58ce3a707a2f5be041842f8a1e4eb4c54dd72e865eb in /nats-server 
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 20:16:33 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 20:16:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 20:16:33 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 20:16:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:68043f4483bff82380b8666c025686881f5483ff754784192f65aa4ec9b662fe`  
		Last Modified: Mon, 07 Aug 2023 20:17:27 GMT  
		Size: 4.9 MB (4924065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0443d8f0ff2c43f481bd49043e2c13423203b3a99754a3baff7df20850bf0e56`  
		Last Modified: Mon, 07 Aug 2023 20:17:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24cb726cdaa647f5307f6d5fa448b299535141c96367b79636f23597407b5071
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4734399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b2f013bc2559b3a905b049fd4b09738b17a4c87d62bed5a1830c6a6e13b1cda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:815b9c4a7d715138f02171cd656c9e8dc6d80e72107c92661c99f6dd24ae2721 in /nats-server 
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:44:14 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:44:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:44:14 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:44:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07116324214b64589e3a471932fe7f6b892068a7cd9cf9bb72a8ea25f8a92200`  
		Last Modified: Mon, 07 Aug 2023 19:44:57 GMT  
		Size: 4.7 MB (4733893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615975e7d25e46607f561d13c4c244d070bb41701a0ac2103df98dcb33e8a4eb`  
		Last Modified: Mon, 07 Aug 2023 19:44:56 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:3959865fd1e3f0b07b7933b6e4772490b619811c09074cfe6fd00985b6614f83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:nanoserver` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:d8a94368172a3df5204943029b32d7b56dda869dadef4983129598ed86fcec67
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109707647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b1b071e5cf657d3db4c3347053329658550fdb8b09ae38a2618af5b119a8565`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 10 Aug 2023 02:34:53 GMT
RUN cmd /S /C #(nop) COPY file:3b8a3a4f656cc66920d77ff06f41851caa37056073cec32caf7e7024bea62100 in C:\nats-server.exe 
# Thu, 10 Aug 2023 02:34:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 10 Aug 2023 02:34:56 GMT
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
	-	`sha256:6810a6f695e6275423db76be5637667297faaa666b58a9658e1690efe300b007`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 5.2 MB (5242246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fbe96bd125f3ebe2f71079f2d8c4ca1d226d4aa3de1dd2a0fefb0e50421464`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c6c360e7d8fa0f4858a220d96a5d13e7c65c195bb8513191b47c1d3b0c6b91`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3db71fcfd8d9cd70e2947e60d0f27dee2449c365fcd7dde18997017f1f7a443`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112aff03752bdfd32ed33505dc8c488a27bdc249bd506edd30af3d47c0d9b4a2`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:3959865fd1e3f0b07b7933b6e4772490b619811c09074cfe6fd00985b6614f83
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:d8a94368172a3df5204943029b32d7b56dda869dadef4983129598ed86fcec67
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.7 MB (109707647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b1b071e5cf657d3db4c3347053329658550fdb8b09ae38a2618af5b119a8565`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 02:34:52 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 10 Aug 2023 02:34:53 GMT
RUN cmd /S /C #(nop) COPY file:3b8a3a4f656cc66920d77ff06f41851caa37056073cec32caf7e7024bea62100 in C:\nats-server.exe 
# Thu, 10 Aug 2023 02:34:54 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 10 Aug 2023 02:34:55 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 10 Aug 2023 02:34:56 GMT
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
	-	`sha256:6810a6f695e6275423db76be5637667297faaa666b58a9658e1690efe300b007`  
		Last Modified: Thu, 10 Aug 2023 02:35:37 GMT  
		Size: 5.2 MB (5242246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9fbe96bd125f3ebe2f71079f2d8c4ca1d226d4aa3de1dd2a0fefb0e50421464`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.7 KB (1702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c6c360e7d8fa0f4858a220d96a5d13e7c65c195bb8513191b47c1d3b0c6b91`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3db71fcfd8d9cd70e2947e60d0f27dee2449c365fcd7dde18997017f1f7a443`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.1 KB (1063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112aff03752bdfd32ed33505dc8c488a27bdc249bd506edd30af3d47c0d9b4a2`  
		Last Modified: Thu, 10 Aug 2023 02:35:35 GMT  
		Size: 1.0 KB (1027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:3208778cf6c64114c84d0227bfd6fb282f1ba86b85f25c46c410c9e97b3a33ca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:cf96338e314ee46e307626e8936dc31b9ef7c67e299b29b7753896d11b52fe8e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5170255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5455cadbb1bd4919947f5a918491add0f2a8fe5d9aa4a801ca79a4ac8fb308f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:26:10 GMT
COPY file:975a38b1520c81a5e1d0876325548b4aefe0036b6deee1ae7ee20db6abbcc080 in /nats-server 
# Mon, 07 Aug 2023 19:26:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:26:11 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:26:11 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:26:11 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:26:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc02d5ba29398595681917073dcd141022b8ad8d0da9a18b6f5752e56c86ceea`  
		Last Modified: Mon, 07 Aug 2023 19:26:56 GMT  
		Size: 5.2 MB (5169747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d9457cd0af5e7125dfe4a44e1d6d003e2bdaf42da9d1c5f7b313069a145e639`  
		Last Modified: Mon, 07 Aug 2023 19:26:55 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:3a3792aaaf193e57879f3594e95501c1372bd2a537965db2bc68fd85c13b8cb8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4932529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966d4a644152a12918ae66827a94561e477b28d10bd2698612566a5c989612f1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:447be8988a65ae095af689a396d155107ebc910fe545508c6e6af6f1c2d2c4d4 in /nats-server 
# Mon, 07 Aug 2023 19:50:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:50:31 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:50:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:50:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:50:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:590d3f4a49d783a9889465cc7862cf43dc4d3a60e0fb075544618efee1ef93e1`  
		Last Modified: Mon, 07 Aug 2023 19:51:13 GMT  
		Size: 4.9 MB (4932022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901e46e20099bb53f1d1b41e9f1cbf04d9af77173e45873723bd9d7825fbbcf0`  
		Last Modified: Mon, 07 Aug 2023 19:51:12 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:3be04f93d99a8e23e99fff2608d9c0d76a4ee2c9c301441f57a2d0b9225c16e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4924573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec722342be0e9d946cb8ac26674a30ff2854116e2e8e1ba75461b3f90d97ecc8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:a28d4beb7d3acaa71be2e58ce3a707a2f5be041842f8a1e4eb4c54dd72e865eb in /nats-server 
# Mon, 07 Aug 2023 20:16:32 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 20:16:33 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 20:16:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 20:16:33 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 20:16:33 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:68043f4483bff82380b8666c025686881f5483ff754784192f65aa4ec9b662fe`  
		Last Modified: Mon, 07 Aug 2023 20:17:27 GMT  
		Size: 4.9 MB (4924065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0443d8f0ff2c43f481bd49043e2c13423203b3a99754a3baff7df20850bf0e56`  
		Last Modified: Mon, 07 Aug 2023 20:17:26 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24cb726cdaa647f5307f6d5fa448b299535141c96367b79636f23597407b5071
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4734399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b2f013bc2559b3a905b049fd4b09738b17a4c87d62bed5a1830c6a6e13b1cda`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:815b9c4a7d715138f02171cd656c9e8dc6d80e72107c92661c99f6dd24ae2721 in /nats-server 
# Mon, 07 Aug 2023 19:44:14 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 07 Aug 2023 19:44:14 GMT
EXPOSE 4222 6222 8222
# Mon, 07 Aug 2023 19:44:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 07 Aug 2023 19:44:14 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 07 Aug 2023 19:44:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:07116324214b64589e3a471932fe7f6b892068a7cd9cf9bb72a8ea25f8a92200`  
		Last Modified: Mon, 07 Aug 2023 19:44:57 GMT  
		Size: 4.7 MB (4733893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615975e7d25e46607f561d13c4c244d070bb41701a0ac2103df98dcb33e8a4eb`  
		Last Modified: Mon, 07 Aug 2023 19:44:56 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:6a5048505a376ddee83a546a4c677bd2c62eaf943530ea64bc946e77b092500c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:windowsservercore` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:df85f652123fd850bc088bf1796ad63e262c83117ef33c913c2324c329e83281
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2001923911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba49e1850a02235e7b24a350ba3483aa40adb3e25011cf8af425be0f74d9bb21`
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
# Thu, 10 Aug 2023 02:32:09 GMT
ENV NATS_SERVER=2.9.21
# Thu, 10 Aug 2023 02:32:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.21/nats-server-v2.9.21-windows-amd64.zip
# Thu, 10 Aug 2023 02:32:11 GMT
ENV NATS_SERVER_SHASUM=43df40bcf81e819e3467a31c548643439d4200486f3032c61ae4b134243f8796
# Thu, 10 Aug 2023 02:33:09 GMT
RUN Set-PSDebug -Trace 2
# Thu, 10 Aug 2023 02:34:42 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 10 Aug 2023 02:34:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 10 Aug 2023 02:34:44 GMT
EXPOSE 4222 6222 8222
# Thu, 10 Aug 2023 02:34:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 10 Aug 2023 02:34:45 GMT
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
	-	`sha256:8065a1cb0e804bbb19260f95fcb2ee724ea73de1da4df8e9744f6498cec33d62`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5638bc45d3356ae277d06dab7b839bf52e16bc50a37408b0de976cebfcd1ab`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc44a5e39ba10538d5f0af74a7c7c00bb731116d9f5f8f19b9469e2464baf901`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98483cb493b32b2587f35850b72b5beb7a5354034943519da2056a8b88a51036`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 242.8 KB (242767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7678609a7e25485895fffda9b5eea9f940ffc5e5e34155de64f2933803428c0e`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 5.7 MB (5712861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b6362b379d0e5ed852e577058ae198521bd47c70a6654e5bdd24a5fbc7f326`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79936c5c24a0ca205db9a615d4c0113a2e3093ae64cdabc9a8b1fa930327830c`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca71b03ad3cfece28d778d224d9c61ca3dbea97dc6761af0d411ddb0275f965d`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484f29887b314709fa52867baf4fc140ec7488361c38d1811854c07d682c1451`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:6a5048505a376ddee83a546a4c677bd2c62eaf943530ea64bc946e77b092500c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull nats@sha256:df85f652123fd850bc088bf1796ad63e262c83117ef33c913c2324c329e83281
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2001923911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba49e1850a02235e7b24a350ba3483aa40adb3e25011cf8af425be0f74d9bb21`
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
# Thu, 10 Aug 2023 02:32:09 GMT
ENV NATS_SERVER=2.9.21
# Thu, 10 Aug 2023 02:32:10 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.21/nats-server-v2.9.21-windows-amd64.zip
# Thu, 10 Aug 2023 02:32:11 GMT
ENV NATS_SERVER_SHASUM=43df40bcf81e819e3467a31c548643439d4200486f3032c61ae4b134243f8796
# Thu, 10 Aug 2023 02:33:09 GMT
RUN Set-PSDebug -Trace 2
# Thu, 10 Aug 2023 02:34:42 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 10 Aug 2023 02:34:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 10 Aug 2023 02:34:44 GMT
EXPOSE 4222 6222 8222
# Thu, 10 Aug 2023 02:34:44 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 10 Aug 2023 02:34:45 GMT
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
	-	`sha256:8065a1cb0e804bbb19260f95fcb2ee724ea73de1da4df8e9744f6498cec33d62`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5638bc45d3356ae277d06dab7b839bf52e16bc50a37408b0de976cebfcd1ab`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc44a5e39ba10538d5f0af74a7c7c00bb731116d9f5f8f19b9469e2464baf901`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98483cb493b32b2587f35850b72b5beb7a5354034943519da2056a8b88a51036`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 242.8 KB (242767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7678609a7e25485895fffda9b5eea9f940ffc5e5e34155de64f2933803428c0e`  
		Last Modified: Thu, 10 Aug 2023 02:35:20 GMT  
		Size: 5.7 MB (5712861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b6362b379d0e5ed852e577058ae198521bd47c70a6654e5bdd24a5fbc7f326`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79936c5c24a0ca205db9a615d4c0113a2e3093ae64cdabc9a8b1fa930327830c`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca71b03ad3cfece28d778d224d9c61ca3dbea97dc6761af0d411ddb0275f965d`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484f29887b314709fa52867baf4fc140ec7488361c38d1811854c07d682c1451`  
		Last Modified: Thu, 10 Aug 2023 02:35:18 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
