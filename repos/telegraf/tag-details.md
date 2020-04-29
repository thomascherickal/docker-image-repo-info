<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `telegraf`

-	[`telegraf:1.12`](#telegraf112)
-	[`telegraf:1.12.6`](#telegraf1126)
-	[`telegraf:1.12.6-alpine`](#telegraf1126-alpine)
-	[`telegraf:1.12-alpine`](#telegraf112-alpine)
-	[`telegraf:1.13`](#telegraf113)
-	[`telegraf:1.13.4`](#telegraf1134)
-	[`telegraf:1.13.4-alpine`](#telegraf1134-alpine)
-	[`telegraf:1.13-alpine`](#telegraf113-alpine)
-	[`telegraf:1.14`](#telegraf114)
-	[`telegraf:1.14.2`](#telegraf1142)
-	[`telegraf:1.14.2-alpine`](#telegraf1142-alpine)
-	[`telegraf:1.14-alpine`](#telegraf114-alpine)
-	[`telegraf:alpine`](#telegrafalpine)
-	[`telegraf:latest`](#telegraflatest)

## `telegraf:1.12`

```console
$ docker pull telegraf@sha256:291bb2e477623cb897c9617555870919b85d1d5288e7adb08ff624e23ec1dcb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.12` - linux; amd64

```console
$ docker pull telegraf@sha256:573a85f2090fc9ea74d05a977fda0937744d5aa221f4b6b439d6a30a00d11cea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.8 MB (97849653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17c625c8fc2f56f5d890ef8ac0819a5ceb2dea5195b474e857a50ee29b48bfc8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 23 Apr 2020 00:22:48 GMT
ADD file:21bf6969c2166c361350c07b1089a1a4b34b7cd3e802a602385d83c49f44a7f6 in / 
# Thu, 23 Apr 2020 00:22:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:59:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 00:59:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 21:42:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 21:42:15 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Apr 2020 21:42:15 GMT
ENV TELEGRAF_VERSION=1.12.6
# Thu, 23 Apr 2020 21:42:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 23 Apr 2020 21:42:19 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 23 Apr 2020 21:42:19 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 23 Apr 2020 21:42:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 21:42:19 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:99760bc62448fbba69f6f0981d09bb4b7532e17362ecfb709141a7195d9b01d3`  
		Last Modified: Thu, 23 Apr 2020 00:27:35 GMT  
		Size: 45.4 MB (45375951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3fa264a7a881e244e7fd3420edda0d550ee3b26ed870f5c021d937497ffd602`  
		Last Modified: Thu, 23 Apr 2020 01:05:50 GMT  
		Size: 10.8 MB (10797279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a222a2af289fc1fe54c037f02e7651e0aead2f81f40cb2885786bfe57aed10a9`  
		Last Modified: Thu, 23 Apr 2020 01:05:48 GMT  
		Size: 4.3 MB (4340174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e55665c9e0e07356546d876ece60fc6716ce709a760ef15c81d71935f374ef3`  
		Last Modified: Thu, 23 Apr 2020 21:43:00 GMT  
		Size: 16.0 MB (15964715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b511841c00a1dc70b635eaba66db076226a14984974a828d6ea12e5e10138ced`  
		Last Modified: Thu, 23 Apr 2020 21:42:56 GMT  
		Size: 2.8 KB (2773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24dd7df668b23879e41e20a5f328fddeeb7442a0058891cfbde09bb67c43b342`  
		Last Modified: Thu, 23 Apr 2020 21:43:01 GMT  
		Size: 21.4 MB (21368576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265105f9c3ae8896ef5dba91451b5a3adab7b279477545d7dbfbe4e1f0330355`  
		Last Modified: Thu, 23 Apr 2020 21:42:56 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.12` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:ae84b16310c59d7838b392d4f9ca519b4abbe63f2a70f3db12e3dc4d7d65ff2d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.5 MB (90521612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:474d85df77363158cf58068dafadbb779e08c1dc4db0ef92ed44ad9e53c3e9c4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 23 Apr 2020 01:07:13 GMT
ADD file:af00fcaffcce2a55b74d080d33cbc9ce5bcf91faf659b887f508c06803fa64bd in / 
# Thu, 23 Apr 2020 01:07:15 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 04:23:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 04:23:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 19:45:44 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 19:45:49 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Apr 2020 19:45:50 GMT
ENV TELEGRAF_VERSION=1.12.6
# Thu, 23 Apr 2020 19:45:56 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 23 Apr 2020 19:45:57 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 23 Apr 2020 19:45:57 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 23 Apr 2020 19:45:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 19:45:59 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4168e46f368afa15fa660f5197fb2946df81a85078c82e37a76d2610fb3999f1`  
		Last Modified: Thu, 23 Apr 2020 01:14:13 GMT  
		Size: 42.1 MB (42101192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bc0e3bfcb00266e5034f08dae24b7862a41a069b0db0c68beb50e66983e602`  
		Last Modified: Thu, 23 Apr 2020 04:34:11 GMT  
		Size: 9.5 MB (9498287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3461f3bce5656c429f5d3faee144de5778a7f01ecd08241211c4badd34a7197b`  
		Last Modified: Thu, 23 Apr 2020 04:34:09 GMT  
		Size: 3.9 MB (3918722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c89366892b85101189243eb93a0a4a9fdbc21b615fc8d3aa603e1b2b6f1695c`  
		Last Modified: Thu, 23 Apr 2020 19:46:59 GMT  
		Size: 14.8 MB (14839164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74aa6be8071a1d0d4fcd5cda97ee3af0b63b759316ed4b27885d63e494e4958`  
		Last Modified: Thu, 23 Apr 2020 19:46:53 GMT  
		Size: 2.8 KB (2801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2633c09cee8b0332f562d64f7fece9958715cf35fbd3ae10834bfc93bea231c`  
		Last Modified: Thu, 23 Apr 2020 19:47:01 GMT  
		Size: 20.2 MB (20161262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f066e978522f9ebcc5161ec6dbe2d88a8055867cab754eac524d0d1a1819219`  
		Last Modified: Thu, 23 Apr 2020 19:46:53 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.12` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:7fca8cf7592930d84f2ea9961ad52fc31769431d1a7cbf1c08af00e332fe29ac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92267780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ff2ee2a471a81bd8d35cd7faeae3de6765c26aaaf254bf8780402cd3e2f65ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 23 Apr 2020 00:58:27 GMT
ADD file:4921b222c4914e830c4c018324aed1904bf1526e01493120ddc9c905373b2673 in / 
# Thu, 23 Apr 2020 00:58:29 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:46:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:46:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 21:23:37 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 21:23:42 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Apr 2020 21:23:43 GMT
ENV TELEGRAF_VERSION=1.12.6
# Thu, 23 Apr 2020 21:23:48 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 23 Apr 2020 21:23:49 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 23 Apr 2020 21:23:50 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 23 Apr 2020 21:23:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 21:23:51 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:decabe2933bfe1939dff94ad523be4904c90e7bea69033943dd32f459d115bab`  
		Last Modified: Thu, 23 Apr 2020 01:05:29 GMT  
		Size: 43.2 MB (43159022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b030385917e3a4847f3280fab5601f7787447be0ac1b9ebdfc5a2b6f966d01`  
		Last Modified: Thu, 23 Apr 2020 03:55:16 GMT  
		Size: 9.7 MB (9748557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3766a78f146d565326c939891f33a75e49f3e5fb549c76d9d19ec413526bb4f0`  
		Last Modified: Thu, 23 Apr 2020 03:55:14 GMT  
		Size: 4.1 MB (4094419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e063050434db1728e621506c3cfad2c7c247fe84e03b3c33470cb1027d09a6`  
		Last Modified: Thu, 23 Apr 2020 21:24:40 GMT  
		Size: 15.5 MB (15530251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a6bf49b82384126f8c9969d6fd716c5ee05b38147cdd2abc4d6599541de512`  
		Last Modified: Thu, 23 Apr 2020 21:24:35 GMT  
		Size: 2.8 KB (2802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c32fde41b9d3de30a22978b5711d34013807a7d4e11f181c33ecf7df68bea4f`  
		Last Modified: Thu, 23 Apr 2020 21:24:42 GMT  
		Size: 19.7 MB (19732545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53fc7a0a12386f7dd92b04e30db8440ae2a6330ef0c6b03a69d776853c4e907c`  
		Last Modified: Thu, 23 Apr 2020 21:24:35 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.12.6`

```console
$ docker pull telegraf@sha256:291bb2e477623cb897c9617555870919b85d1d5288e7adb08ff624e23ec1dcb9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.12.6` - linux; amd64

```console
$ docker pull telegraf@sha256:573a85f2090fc9ea74d05a977fda0937744d5aa221f4b6b439d6a30a00d11cea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.8 MB (97849653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17c625c8fc2f56f5d890ef8ac0819a5ceb2dea5195b474e857a50ee29b48bfc8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 23 Apr 2020 00:22:48 GMT
ADD file:21bf6969c2166c361350c07b1089a1a4b34b7cd3e802a602385d83c49f44a7f6 in / 
# Thu, 23 Apr 2020 00:22:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:59:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 00:59:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 21:42:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 21:42:15 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Apr 2020 21:42:15 GMT
ENV TELEGRAF_VERSION=1.12.6
# Thu, 23 Apr 2020 21:42:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 23 Apr 2020 21:42:19 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 23 Apr 2020 21:42:19 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 23 Apr 2020 21:42:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 21:42:19 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:99760bc62448fbba69f6f0981d09bb4b7532e17362ecfb709141a7195d9b01d3`  
		Last Modified: Thu, 23 Apr 2020 00:27:35 GMT  
		Size: 45.4 MB (45375951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3fa264a7a881e244e7fd3420edda0d550ee3b26ed870f5c021d937497ffd602`  
		Last Modified: Thu, 23 Apr 2020 01:05:50 GMT  
		Size: 10.8 MB (10797279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a222a2af289fc1fe54c037f02e7651e0aead2f81f40cb2885786bfe57aed10a9`  
		Last Modified: Thu, 23 Apr 2020 01:05:48 GMT  
		Size: 4.3 MB (4340174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e55665c9e0e07356546d876ece60fc6716ce709a760ef15c81d71935f374ef3`  
		Last Modified: Thu, 23 Apr 2020 21:43:00 GMT  
		Size: 16.0 MB (15964715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b511841c00a1dc70b635eaba66db076226a14984974a828d6ea12e5e10138ced`  
		Last Modified: Thu, 23 Apr 2020 21:42:56 GMT  
		Size: 2.8 KB (2773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24dd7df668b23879e41e20a5f328fddeeb7442a0058891cfbde09bb67c43b342`  
		Last Modified: Thu, 23 Apr 2020 21:43:01 GMT  
		Size: 21.4 MB (21368576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:265105f9c3ae8896ef5dba91451b5a3adab7b279477545d7dbfbe4e1f0330355`  
		Last Modified: Thu, 23 Apr 2020 21:42:56 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.12.6` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:ae84b16310c59d7838b392d4f9ca519b4abbe63f2a70f3db12e3dc4d7d65ff2d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.5 MB (90521612 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:474d85df77363158cf58068dafadbb779e08c1dc4db0ef92ed44ad9e53c3e9c4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 23 Apr 2020 01:07:13 GMT
ADD file:af00fcaffcce2a55b74d080d33cbc9ce5bcf91faf659b887f508c06803fa64bd in / 
# Thu, 23 Apr 2020 01:07:15 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 04:23:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 04:23:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 19:45:44 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 19:45:49 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Apr 2020 19:45:50 GMT
ENV TELEGRAF_VERSION=1.12.6
# Thu, 23 Apr 2020 19:45:56 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 23 Apr 2020 19:45:57 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 23 Apr 2020 19:45:57 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 23 Apr 2020 19:45:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 19:45:59 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4168e46f368afa15fa660f5197fb2946df81a85078c82e37a76d2610fb3999f1`  
		Last Modified: Thu, 23 Apr 2020 01:14:13 GMT  
		Size: 42.1 MB (42101192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bc0e3bfcb00266e5034f08dae24b7862a41a069b0db0c68beb50e66983e602`  
		Last Modified: Thu, 23 Apr 2020 04:34:11 GMT  
		Size: 9.5 MB (9498287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3461f3bce5656c429f5d3faee144de5778a7f01ecd08241211c4badd34a7197b`  
		Last Modified: Thu, 23 Apr 2020 04:34:09 GMT  
		Size: 3.9 MB (3918722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c89366892b85101189243eb93a0a4a9fdbc21b615fc8d3aa603e1b2b6f1695c`  
		Last Modified: Thu, 23 Apr 2020 19:46:59 GMT  
		Size: 14.8 MB (14839164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74aa6be8071a1d0d4fcd5cda97ee3af0b63b759316ed4b27885d63e494e4958`  
		Last Modified: Thu, 23 Apr 2020 19:46:53 GMT  
		Size: 2.8 KB (2801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2633c09cee8b0332f562d64f7fece9958715cf35fbd3ae10834bfc93bea231c`  
		Last Modified: Thu, 23 Apr 2020 19:47:01 GMT  
		Size: 20.2 MB (20161262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f066e978522f9ebcc5161ec6dbe2d88a8055867cab754eac524d0d1a1819219`  
		Last Modified: Thu, 23 Apr 2020 19:46:53 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.12.6` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:7fca8cf7592930d84f2ea9961ad52fc31769431d1a7cbf1c08af00e332fe29ac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92267780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ff2ee2a471a81bd8d35cd7faeae3de6765c26aaaf254bf8780402cd3e2f65ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 23 Apr 2020 00:58:27 GMT
ADD file:4921b222c4914e830c4c018324aed1904bf1526e01493120ddc9c905373b2673 in / 
# Thu, 23 Apr 2020 00:58:29 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:46:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:46:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 21:23:37 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 21:23:42 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Apr 2020 21:23:43 GMT
ENV TELEGRAF_VERSION=1.12.6
# Thu, 23 Apr 2020 21:23:48 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 23 Apr 2020 21:23:49 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 23 Apr 2020 21:23:50 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 23 Apr 2020 21:23:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 21:23:51 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:decabe2933bfe1939dff94ad523be4904c90e7bea69033943dd32f459d115bab`  
		Last Modified: Thu, 23 Apr 2020 01:05:29 GMT  
		Size: 43.2 MB (43159022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b030385917e3a4847f3280fab5601f7787447be0ac1b9ebdfc5a2b6f966d01`  
		Last Modified: Thu, 23 Apr 2020 03:55:16 GMT  
		Size: 9.7 MB (9748557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3766a78f146d565326c939891f33a75e49f3e5fb549c76d9d19ec413526bb4f0`  
		Last Modified: Thu, 23 Apr 2020 03:55:14 GMT  
		Size: 4.1 MB (4094419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e063050434db1728e621506c3cfad2c7c247fe84e03b3c33470cb1027d09a6`  
		Last Modified: Thu, 23 Apr 2020 21:24:40 GMT  
		Size: 15.5 MB (15530251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a6bf49b82384126f8c9969d6fd716c5ee05b38147cdd2abc4d6599541de512`  
		Last Modified: Thu, 23 Apr 2020 21:24:35 GMT  
		Size: 2.8 KB (2802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c32fde41b9d3de30a22978b5711d34013807a7d4e11f181c33ecf7df68bea4f`  
		Last Modified: Thu, 23 Apr 2020 21:24:42 GMT  
		Size: 19.7 MB (19732545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53fc7a0a12386f7dd92b04e30db8440ae2a6330ef0c6b03a69d776853c4e907c`  
		Last Modified: Thu, 23 Apr 2020 21:24:35 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.12.6-alpine`

```console
$ docker pull telegraf@sha256:88f59aacd3dbef010bdd5cb6527e852e933a1b79a2e907e61666bb0f8e92013a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:1.12.6-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:7b0c8a6d7cd0a4ba7646b3c5926ef44a490a3a8d4e9f89cca2889a928d70a822
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27854316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2e6a0fe70f163b3ba1c3df5c28d7f0dbdda50ae967cf10b79e5b28a28623082`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:24:06 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Fri, 24 Apr 2020 14:24:06 GMT
ENV TELEGRAF_VERSION=1.12.6
# Fri, 24 Apr 2020 14:24:10 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/telegraf.conf /etc/telegraf/ &&     chmod +x /usr/src/telegraf*/* &&     cp -a /usr/src/telegraf*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 14:24:10 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 24 Apr 2020 14:24:10 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Fri, 24 Apr 2020 14:24:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:24:11 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321996f3080d1a7516b5914e27460b495eb04950d0190554844f395e7be9c793`  
		Last Modified: Fri, 24 Apr 2020 14:16:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21ceaab89b626cc487c744b86ea671176e8adf45ada4605d74c66278d136829`  
		Last Modified: Fri, 24 Apr 2020 14:24:49 GMT  
		Size: 3.7 MB (3720297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d142ff75baa0a44652c2874af91eb8b22457112d6f9a3ccabc2199ba2d97c99`  
		Last Modified: Fri, 24 Apr 2020 14:24:52 GMT  
		Size: 21.4 MB (21360269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce28b0bfe86cf8633862376618d78142310380ab980d43015959151806e28958`  
		Last Modified: Fri, 24 Apr 2020 14:24:48 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.12-alpine`

```console
$ docker pull telegraf@sha256:88f59aacd3dbef010bdd5cb6527e852e933a1b79a2e907e61666bb0f8e92013a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:1.12-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:7b0c8a6d7cd0a4ba7646b3c5926ef44a490a3a8d4e9f89cca2889a928d70a822
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27854316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2e6a0fe70f163b3ba1c3df5c28d7f0dbdda50ae967cf10b79e5b28a28623082`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:24:06 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Fri, 24 Apr 2020 14:24:06 GMT
ENV TELEGRAF_VERSION=1.12.6
# Fri, 24 Apr 2020 14:24:10 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/telegraf.conf /etc/telegraf/ &&     chmod +x /usr/src/telegraf*/* &&     cp -a /usr/src/telegraf*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 14:24:10 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 24 Apr 2020 14:24:10 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Fri, 24 Apr 2020 14:24:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:24:11 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321996f3080d1a7516b5914e27460b495eb04950d0190554844f395e7be9c793`  
		Last Modified: Fri, 24 Apr 2020 14:16:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21ceaab89b626cc487c744b86ea671176e8adf45ada4605d74c66278d136829`  
		Last Modified: Fri, 24 Apr 2020 14:24:49 GMT  
		Size: 3.7 MB (3720297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d142ff75baa0a44652c2874af91eb8b22457112d6f9a3ccabc2199ba2d97c99`  
		Last Modified: Fri, 24 Apr 2020 14:24:52 GMT  
		Size: 21.4 MB (21360269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce28b0bfe86cf8633862376618d78142310380ab980d43015959151806e28958`  
		Last Modified: Fri, 24 Apr 2020 14:24:48 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.13`

```console
$ docker pull telegraf@sha256:4a3ef9bbb3552b9472b482913a09c5d2f0f15d7eea6a308d89b23e9787245ab2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.13` - linux; amd64

```console
$ docker pull telegraf@sha256:329ebe78ded71e21795ce468ce45b55719796464ac8a7fcad8c96d68df891721
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.8 MB (96792871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:470734f6bd56a9a94c7f0a2ea3bed38c51fb1f9dc383e54b519dd6183d2fa325`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 23 Apr 2020 00:22:48 GMT
ADD file:21bf6969c2166c361350c07b1089a1a4b34b7cd3e802a602385d83c49f44a7f6 in / 
# Thu, 23 Apr 2020 00:22:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:59:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 00:59:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 21:42:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 21:42:15 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Apr 2020 21:42:27 GMT
ENV TELEGRAF_VERSION=1.13.4
# Thu, 23 Apr 2020 21:42:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 23 Apr 2020 21:42:30 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 23 Apr 2020 21:42:30 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 23 Apr 2020 21:42:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 21:42:31 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:99760bc62448fbba69f6f0981d09bb4b7532e17362ecfb709141a7195d9b01d3`  
		Last Modified: Thu, 23 Apr 2020 00:27:35 GMT  
		Size: 45.4 MB (45375951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3fa264a7a881e244e7fd3420edda0d550ee3b26ed870f5c021d937497ffd602`  
		Last Modified: Thu, 23 Apr 2020 01:05:50 GMT  
		Size: 10.8 MB (10797279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a222a2af289fc1fe54c037f02e7651e0aead2f81f40cb2885786bfe57aed10a9`  
		Last Modified: Thu, 23 Apr 2020 01:05:48 GMT  
		Size: 4.3 MB (4340174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e55665c9e0e07356546d876ece60fc6716ce709a760ef15c81d71935f374ef3`  
		Last Modified: Thu, 23 Apr 2020 21:43:00 GMT  
		Size: 16.0 MB (15964715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b511841c00a1dc70b635eaba66db076226a14984974a828d6ea12e5e10138ced`  
		Last Modified: Thu, 23 Apr 2020 21:42:56 GMT  
		Size: 2.8 KB (2773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a765cd97365516b219ea45a237faedf8615e3fa6c7a5f83ebe7e011f76f781a`  
		Last Modified: Thu, 23 Apr 2020 21:43:11 GMT  
		Size: 20.3 MB (20311794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a301355003d2b98ae04d539f56d1b1220dff1b1370af4b57688326e73f298cf9`  
		Last Modified: Thu, 23 Apr 2020 21:43:06 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.13` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:6d081a200d0c15dddc5d762e3ae18369beea05b1e936d94c5a0b6f7d84171e82
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.4 MB (89413376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a6ff7289290506608bf5da6ac7e10e8b6485e43db1e90b71bd7f7f9d2d2afee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 23 Apr 2020 01:07:13 GMT
ADD file:af00fcaffcce2a55b74d080d33cbc9ce5bcf91faf659b887f508c06803fa64bd in / 
# Thu, 23 Apr 2020 01:07:15 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 04:23:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 04:23:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 19:45:44 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 19:45:49 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Apr 2020 19:46:08 GMT
ENV TELEGRAF_VERSION=1.13.4
# Thu, 23 Apr 2020 19:46:17 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 23 Apr 2020 19:46:18 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 23 Apr 2020 19:46:19 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 23 Apr 2020 19:46:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 19:46:23 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4168e46f368afa15fa660f5197fb2946df81a85078c82e37a76d2610fb3999f1`  
		Last Modified: Thu, 23 Apr 2020 01:14:13 GMT  
		Size: 42.1 MB (42101192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bc0e3bfcb00266e5034f08dae24b7862a41a069b0db0c68beb50e66983e602`  
		Last Modified: Thu, 23 Apr 2020 04:34:11 GMT  
		Size: 9.5 MB (9498287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3461f3bce5656c429f5d3faee144de5778a7f01ecd08241211c4badd34a7197b`  
		Last Modified: Thu, 23 Apr 2020 04:34:09 GMT  
		Size: 3.9 MB (3918722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c89366892b85101189243eb93a0a4a9fdbc21b615fc8d3aa603e1b2b6f1695c`  
		Last Modified: Thu, 23 Apr 2020 19:46:59 GMT  
		Size: 14.8 MB (14839164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74aa6be8071a1d0d4fcd5cda97ee3af0b63b759316ed4b27885d63e494e4958`  
		Last Modified: Thu, 23 Apr 2020 19:46:53 GMT  
		Size: 2.8 KB (2801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222bd049d7eb3bd1a3d12b54346887f8d699ab016ef3e3e2b2ff1b90142e68c4`  
		Last Modified: Thu, 23 Apr 2020 19:47:15 GMT  
		Size: 19.1 MB (19053025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cd56930cb02c0fba92777a2033941fc62efa6908cbe57fa773570f411f1b64`  
		Last Modified: Thu, 23 Apr 2020 19:47:09 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.13` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:bd28ac3ca3d740679e40eb52040b40fcd25172b69f7a9bcb498ffa76cd2dfe69
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91240553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aea9dc8b0171010a43c78a4ea893c809eeed78e7b2549b561873116b12314fbf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 23 Apr 2020 00:58:27 GMT
ADD file:4921b222c4914e830c4c018324aed1904bf1526e01493120ddc9c905373b2673 in / 
# Thu, 23 Apr 2020 00:58:29 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:46:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:46:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 21:23:37 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 21:23:42 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Apr 2020 21:24:01 GMT
ENV TELEGRAF_VERSION=1.13.4
# Thu, 23 Apr 2020 21:24:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 23 Apr 2020 21:24:07 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 23 Apr 2020 21:24:08 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 23 Apr 2020 21:24:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 21:24:09 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:decabe2933bfe1939dff94ad523be4904c90e7bea69033943dd32f459d115bab`  
		Last Modified: Thu, 23 Apr 2020 01:05:29 GMT  
		Size: 43.2 MB (43159022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b030385917e3a4847f3280fab5601f7787447be0ac1b9ebdfc5a2b6f966d01`  
		Last Modified: Thu, 23 Apr 2020 03:55:16 GMT  
		Size: 9.7 MB (9748557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3766a78f146d565326c939891f33a75e49f3e5fb549c76d9d19ec413526bb4f0`  
		Last Modified: Thu, 23 Apr 2020 03:55:14 GMT  
		Size: 4.1 MB (4094419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e063050434db1728e621506c3cfad2c7c247fe84e03b3c33470cb1027d09a6`  
		Last Modified: Thu, 23 Apr 2020 21:24:40 GMT  
		Size: 15.5 MB (15530251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a6bf49b82384126f8c9969d6fd716c5ee05b38147cdd2abc4d6599541de512`  
		Last Modified: Thu, 23 Apr 2020 21:24:35 GMT  
		Size: 2.8 KB (2802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85b15b696661dc3f6e03db3fde2621c1075cb448e493059d982338b85d26755`  
		Last Modified: Thu, 23 Apr 2020 21:24:55 GMT  
		Size: 18.7 MB (18705318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58337c98af1583a3fbc0b7106185489f625168ab98820382c63944a862e3ffcf`  
		Last Modified: Thu, 23 Apr 2020 21:24:49 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.13.4`

```console
$ docker pull telegraf@sha256:4a3ef9bbb3552b9472b482913a09c5d2f0f15d7eea6a308d89b23e9787245ab2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.13.4` - linux; amd64

```console
$ docker pull telegraf@sha256:329ebe78ded71e21795ce468ce45b55719796464ac8a7fcad8c96d68df891721
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.8 MB (96792871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:470734f6bd56a9a94c7f0a2ea3bed38c51fb1f9dc383e54b519dd6183d2fa325`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 23 Apr 2020 00:22:48 GMT
ADD file:21bf6969c2166c361350c07b1089a1a4b34b7cd3e802a602385d83c49f44a7f6 in / 
# Thu, 23 Apr 2020 00:22:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:59:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 00:59:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 21:42:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 21:42:15 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Apr 2020 21:42:27 GMT
ENV TELEGRAF_VERSION=1.13.4
# Thu, 23 Apr 2020 21:42:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 23 Apr 2020 21:42:30 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 23 Apr 2020 21:42:30 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 23 Apr 2020 21:42:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 21:42:31 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:99760bc62448fbba69f6f0981d09bb4b7532e17362ecfb709141a7195d9b01d3`  
		Last Modified: Thu, 23 Apr 2020 00:27:35 GMT  
		Size: 45.4 MB (45375951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3fa264a7a881e244e7fd3420edda0d550ee3b26ed870f5c021d937497ffd602`  
		Last Modified: Thu, 23 Apr 2020 01:05:50 GMT  
		Size: 10.8 MB (10797279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a222a2af289fc1fe54c037f02e7651e0aead2f81f40cb2885786bfe57aed10a9`  
		Last Modified: Thu, 23 Apr 2020 01:05:48 GMT  
		Size: 4.3 MB (4340174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e55665c9e0e07356546d876ece60fc6716ce709a760ef15c81d71935f374ef3`  
		Last Modified: Thu, 23 Apr 2020 21:43:00 GMT  
		Size: 16.0 MB (15964715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b511841c00a1dc70b635eaba66db076226a14984974a828d6ea12e5e10138ced`  
		Last Modified: Thu, 23 Apr 2020 21:42:56 GMT  
		Size: 2.8 KB (2773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a765cd97365516b219ea45a237faedf8615e3fa6c7a5f83ebe7e011f76f781a`  
		Last Modified: Thu, 23 Apr 2020 21:43:11 GMT  
		Size: 20.3 MB (20311794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a301355003d2b98ae04d539f56d1b1220dff1b1370af4b57688326e73f298cf9`  
		Last Modified: Thu, 23 Apr 2020 21:43:06 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.13.4` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:6d081a200d0c15dddc5d762e3ae18369beea05b1e936d94c5a0b6f7d84171e82
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.4 MB (89413376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a6ff7289290506608bf5da6ac7e10e8b6485e43db1e90b71bd7f7f9d2d2afee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 23 Apr 2020 01:07:13 GMT
ADD file:af00fcaffcce2a55b74d080d33cbc9ce5bcf91faf659b887f508c06803fa64bd in / 
# Thu, 23 Apr 2020 01:07:15 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 04:23:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 04:23:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 19:45:44 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 19:45:49 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Apr 2020 19:46:08 GMT
ENV TELEGRAF_VERSION=1.13.4
# Thu, 23 Apr 2020 19:46:17 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 23 Apr 2020 19:46:18 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 23 Apr 2020 19:46:19 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 23 Apr 2020 19:46:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 19:46:23 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4168e46f368afa15fa660f5197fb2946df81a85078c82e37a76d2610fb3999f1`  
		Last Modified: Thu, 23 Apr 2020 01:14:13 GMT  
		Size: 42.1 MB (42101192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bc0e3bfcb00266e5034f08dae24b7862a41a069b0db0c68beb50e66983e602`  
		Last Modified: Thu, 23 Apr 2020 04:34:11 GMT  
		Size: 9.5 MB (9498287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3461f3bce5656c429f5d3faee144de5778a7f01ecd08241211c4badd34a7197b`  
		Last Modified: Thu, 23 Apr 2020 04:34:09 GMT  
		Size: 3.9 MB (3918722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c89366892b85101189243eb93a0a4a9fdbc21b615fc8d3aa603e1b2b6f1695c`  
		Last Modified: Thu, 23 Apr 2020 19:46:59 GMT  
		Size: 14.8 MB (14839164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74aa6be8071a1d0d4fcd5cda97ee3af0b63b759316ed4b27885d63e494e4958`  
		Last Modified: Thu, 23 Apr 2020 19:46:53 GMT  
		Size: 2.8 KB (2801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222bd049d7eb3bd1a3d12b54346887f8d699ab016ef3e3e2b2ff1b90142e68c4`  
		Last Modified: Thu, 23 Apr 2020 19:47:15 GMT  
		Size: 19.1 MB (19053025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cd56930cb02c0fba92777a2033941fc62efa6908cbe57fa773570f411f1b64`  
		Last Modified: Thu, 23 Apr 2020 19:47:09 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.13.4` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:bd28ac3ca3d740679e40eb52040b40fcd25172b69f7a9bcb498ffa76cd2dfe69
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.2 MB (91240553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aea9dc8b0171010a43c78a4ea893c809eeed78e7b2549b561873116b12314fbf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 23 Apr 2020 00:58:27 GMT
ADD file:4921b222c4914e830c4c018324aed1904bf1526e01493120ddc9c905373b2673 in / 
# Thu, 23 Apr 2020 00:58:29 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:46:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:46:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 21:23:37 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 21:23:42 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Apr 2020 21:24:01 GMT
ENV TELEGRAF_VERSION=1.13.4
# Thu, 23 Apr 2020 21:24:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 23 Apr 2020 21:24:07 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 23 Apr 2020 21:24:08 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 23 Apr 2020 21:24:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 21:24:09 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:decabe2933bfe1939dff94ad523be4904c90e7bea69033943dd32f459d115bab`  
		Last Modified: Thu, 23 Apr 2020 01:05:29 GMT  
		Size: 43.2 MB (43159022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b030385917e3a4847f3280fab5601f7787447be0ac1b9ebdfc5a2b6f966d01`  
		Last Modified: Thu, 23 Apr 2020 03:55:16 GMT  
		Size: 9.7 MB (9748557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3766a78f146d565326c939891f33a75e49f3e5fb549c76d9d19ec413526bb4f0`  
		Last Modified: Thu, 23 Apr 2020 03:55:14 GMT  
		Size: 4.1 MB (4094419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e063050434db1728e621506c3cfad2c7c247fe84e03b3c33470cb1027d09a6`  
		Last Modified: Thu, 23 Apr 2020 21:24:40 GMT  
		Size: 15.5 MB (15530251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a6bf49b82384126f8c9969d6fd716c5ee05b38147cdd2abc4d6599541de512`  
		Last Modified: Thu, 23 Apr 2020 21:24:35 GMT  
		Size: 2.8 KB (2802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85b15b696661dc3f6e03db3fde2621c1075cb448e493059d982338b85d26755`  
		Last Modified: Thu, 23 Apr 2020 21:24:55 GMT  
		Size: 18.7 MB (18705318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58337c98af1583a3fbc0b7106185489f625168ab98820382c63944a862e3ffcf`  
		Last Modified: Thu, 23 Apr 2020 21:24:49 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.13.4-alpine`

```console
$ docker pull telegraf@sha256:69b94db3382157ac83f038c214ed6ff6e45d66d98674729a77bdf61aae3ed24c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:1.13.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:b63949253dc27196cc56d2c4b37725ee788f75e275ade9d313843c57aa77a628
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.8 MB (26785588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48c9cb07cabc64d9937b921e995328bea356ab7f7c78ad2604199b5809a29d07`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:24:06 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Fri, 24 Apr 2020 14:24:18 GMT
ENV TELEGRAF_VERSION=1.13.4
# Fri, 24 Apr 2020 14:24:22 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/telegraf.conf /etc/telegraf/ &&     chmod +x /usr/src/telegraf*/* &&     cp -a /usr/src/telegraf*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 14:24:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 24 Apr 2020 14:24:22 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Fri, 24 Apr 2020 14:24:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:24:23 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321996f3080d1a7516b5914e27460b495eb04950d0190554844f395e7be9c793`  
		Last Modified: Fri, 24 Apr 2020 14:16:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21ceaab89b626cc487c744b86ea671176e8adf45ada4605d74c66278d136829`  
		Last Modified: Fri, 24 Apr 2020 14:24:49 GMT  
		Size: 3.7 MB (3720297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf519af12b10fd075a5f8db5b1c74f3c911ecd7bb59aa1ffddfbb11da4573d7`  
		Last Modified: Fri, 24 Apr 2020 14:25:00 GMT  
		Size: 20.3 MB (20291543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd64901ca1cf1ed9041856bd9403f3a0a4e3d6f5ece8d5d96a79dd24bf7fc18`  
		Last Modified: Fri, 24 Apr 2020 14:24:56 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.13-alpine`

```console
$ docker pull telegraf@sha256:69b94db3382157ac83f038c214ed6ff6e45d66d98674729a77bdf61aae3ed24c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:1.13-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:b63949253dc27196cc56d2c4b37725ee788f75e275ade9d313843c57aa77a628
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.8 MB (26785588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48c9cb07cabc64d9937b921e995328bea356ab7f7c78ad2604199b5809a29d07`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:24:06 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Fri, 24 Apr 2020 14:24:18 GMT
ENV TELEGRAF_VERSION=1.13.4
# Fri, 24 Apr 2020 14:24:22 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/telegraf.conf /etc/telegraf/ &&     chmod +x /usr/src/telegraf*/* &&     cp -a /usr/src/telegraf*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 14:24:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 24 Apr 2020 14:24:22 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Fri, 24 Apr 2020 14:24:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:24:23 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321996f3080d1a7516b5914e27460b495eb04950d0190554844f395e7be9c793`  
		Last Modified: Fri, 24 Apr 2020 14:16:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21ceaab89b626cc487c744b86ea671176e8adf45ada4605d74c66278d136829`  
		Last Modified: Fri, 24 Apr 2020 14:24:49 GMT  
		Size: 3.7 MB (3720297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf519af12b10fd075a5f8db5b1c74f3c911ecd7bb59aa1ffddfbb11da4573d7`  
		Last Modified: Fri, 24 Apr 2020 14:25:00 GMT  
		Size: 20.3 MB (20291543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd64901ca1cf1ed9041856bd9403f3a0a4e3d6f5ece8d5d96a79dd24bf7fc18`  
		Last Modified: Fri, 24 Apr 2020 14:24:56 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.14`

```console
$ docker pull telegraf@sha256:f6c959c3227f5b6521dc57e0355aa2d3256e39a191261e11588508ed3428f137
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.14` - linux; amd64

```console
$ docker pull telegraf@sha256:db9ddd787c33aed7a92cae7ff042c6a9609405e961e2589331df8899eac85a40
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.9 MB (97901818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d12ef0c09ccf5f26af0f760e9cb2531782bd5dafeee85c1854a4c1dc274e44c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 23 Apr 2020 00:22:48 GMT
ADD file:21bf6969c2166c361350c07b1089a1a4b34b7cd3e802a602385d83c49f44a7f6 in / 
# Thu, 23 Apr 2020 00:22:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:59:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 00:59:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 21:42:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 21:42:15 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Apr 2020 21:42:38 GMT
ENV TELEGRAF_VERSION=1.14.1
# Thu, 23 Apr 2020 21:42:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 23 Apr 2020 21:42:42 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 23 Apr 2020 21:42:42 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 23 Apr 2020 21:42:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 21:42:42 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:99760bc62448fbba69f6f0981d09bb4b7532e17362ecfb709141a7195d9b01d3`  
		Last Modified: Thu, 23 Apr 2020 00:27:35 GMT  
		Size: 45.4 MB (45375951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3fa264a7a881e244e7fd3420edda0d550ee3b26ed870f5c021d937497ffd602`  
		Last Modified: Thu, 23 Apr 2020 01:05:50 GMT  
		Size: 10.8 MB (10797279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a222a2af289fc1fe54c037f02e7651e0aead2f81f40cb2885786bfe57aed10a9`  
		Last Modified: Thu, 23 Apr 2020 01:05:48 GMT  
		Size: 4.3 MB (4340174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e55665c9e0e07356546d876ece60fc6716ce709a760ef15c81d71935f374ef3`  
		Last Modified: Thu, 23 Apr 2020 21:43:00 GMT  
		Size: 16.0 MB (15964715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b511841c00a1dc70b635eaba66db076226a14984974a828d6ea12e5e10138ced`  
		Last Modified: Thu, 23 Apr 2020 21:42:56 GMT  
		Size: 2.8 KB (2773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e412a1c29e41dd4673ebd026157db07b059b7a4fed6f8de3f8b530a21cbf00f`  
		Last Modified: Thu, 23 Apr 2020 21:43:20 GMT  
		Size: 21.4 MB (21420740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1067933cce2388d5b0bc901ab755d7be219d092463555fd857b681b30c3041`  
		Last Modified: Thu, 23 Apr 2020 21:43:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.14` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:a7dce1f73a4da00e5059a834d09b489f773418656e38dcf2b3024cde452e5841
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.5 MB (90490056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13d4e06057f2b37d4fb30349bd239d8e707a953144ee243986eacd6c0ebdf198`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 23 Apr 2020 01:07:13 GMT
ADD file:af00fcaffcce2a55b74d080d33cbc9ce5bcf91faf659b887f508c06803fa64bd in / 
# Thu, 23 Apr 2020 01:07:15 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 04:23:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 04:23:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 19:45:44 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 19:45:49 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Apr 2020 19:46:29 GMT
ENV TELEGRAF_VERSION=1.14.1
# Thu, 23 Apr 2020 19:46:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 23 Apr 2020 19:46:39 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 23 Apr 2020 19:46:40 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 23 Apr 2020 19:46:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 19:46:41 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4168e46f368afa15fa660f5197fb2946df81a85078c82e37a76d2610fb3999f1`  
		Last Modified: Thu, 23 Apr 2020 01:14:13 GMT  
		Size: 42.1 MB (42101192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bc0e3bfcb00266e5034f08dae24b7862a41a069b0db0c68beb50e66983e602`  
		Last Modified: Thu, 23 Apr 2020 04:34:11 GMT  
		Size: 9.5 MB (9498287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3461f3bce5656c429f5d3faee144de5778a7f01ecd08241211c4badd34a7197b`  
		Last Modified: Thu, 23 Apr 2020 04:34:09 GMT  
		Size: 3.9 MB (3918722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c89366892b85101189243eb93a0a4a9fdbc21b615fc8d3aa603e1b2b6f1695c`  
		Last Modified: Thu, 23 Apr 2020 19:46:59 GMT  
		Size: 14.8 MB (14839164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74aa6be8071a1d0d4fcd5cda97ee3af0b63b759316ed4b27885d63e494e4958`  
		Last Modified: Thu, 23 Apr 2020 19:46:53 GMT  
		Size: 2.8 KB (2801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1668ff82c5768d9f7c77063b65d5396a641115f6052533b927c89becb2b030f3`  
		Last Modified: Thu, 23 Apr 2020 19:47:31 GMT  
		Size: 20.1 MB (20129704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3fde1a42a7bcfa704a405e3f4790ad507244e487583b74dff427d0d7be7f860`  
		Last Modified: Thu, 23 Apr 2020 19:47:23 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.14` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:e0e9994ef1393b3b18f01253cf333f7396a79eae0d0d36692d8a274bb656a9bd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92257106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c08609e65ef6813198e2378f60210aca502ec5d4b4b6242fd15d204cda6b465`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 23 Apr 2020 00:58:27 GMT
ADD file:4921b222c4914e830c4c018324aed1904bf1526e01493120ddc9c905373b2673 in / 
# Thu, 23 Apr 2020 00:58:29 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:46:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:46:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 21:23:37 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 21:23:42 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Apr 2020 21:24:15 GMT
ENV TELEGRAF_VERSION=1.14.1
# Thu, 23 Apr 2020 21:24:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 23 Apr 2020 21:24:21 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 23 Apr 2020 21:24:22 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 23 Apr 2020 21:24:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 21:24:23 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:decabe2933bfe1939dff94ad523be4904c90e7bea69033943dd32f459d115bab`  
		Last Modified: Thu, 23 Apr 2020 01:05:29 GMT  
		Size: 43.2 MB (43159022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b030385917e3a4847f3280fab5601f7787447be0ac1b9ebdfc5a2b6f966d01`  
		Last Modified: Thu, 23 Apr 2020 03:55:16 GMT  
		Size: 9.7 MB (9748557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3766a78f146d565326c939891f33a75e49f3e5fb549c76d9d19ec413526bb4f0`  
		Last Modified: Thu, 23 Apr 2020 03:55:14 GMT  
		Size: 4.1 MB (4094419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e063050434db1728e621506c3cfad2c7c247fe84e03b3c33470cb1027d09a6`  
		Last Modified: Thu, 23 Apr 2020 21:24:40 GMT  
		Size: 15.5 MB (15530251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a6bf49b82384126f8c9969d6fd716c5ee05b38147cdd2abc4d6599541de512`  
		Last Modified: Thu, 23 Apr 2020 21:24:35 GMT  
		Size: 2.8 KB (2802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dfa2bc79aad24602f2c690fbcb317d24f3b348e05e7982d21e1dde74c6a796`  
		Last Modified: Thu, 23 Apr 2020 21:25:08 GMT  
		Size: 19.7 MB (19721871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4feb40a14691c117e1ee7ac84afcad6c95c3e3ba24959792fb05adcbb68174e4`  
		Last Modified: Thu, 23 Apr 2020 21:25:02 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.14.2`

```console
$ docker pull telegraf@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `telegraf:1.14.2-alpine`

```console
$ docker pull telegraf@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `telegraf:1.14-alpine`

```console
$ docker pull telegraf@sha256:5a4e168ea396e61a8b853c77b239c34a52a3be61c7110311f567a373557fa0fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:1.14-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:9df10e6ff8b7ee79a0c0ad1c04cc4d85f0f91b7b0d67d8719169888d16eceebb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27909511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:955a6065421ce8267ab0aabea5e76ff6b00b60ea8bf3f76a6a77c7a08a213088`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:24:06 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Fri, 24 Apr 2020 14:24:29 GMT
ENV TELEGRAF_VERSION=1.14.1
# Fri, 24 Apr 2020 14:24:33 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/telegraf.conf /etc/telegraf/ &&     chmod +x /usr/src/telegraf*/* &&     cp -a /usr/src/telegraf*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 14:24:33 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 24 Apr 2020 14:24:34 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Fri, 24 Apr 2020 14:24:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:24:34 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321996f3080d1a7516b5914e27460b495eb04950d0190554844f395e7be9c793`  
		Last Modified: Fri, 24 Apr 2020 14:16:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21ceaab89b626cc487c744b86ea671176e8adf45ada4605d74c66278d136829`  
		Last Modified: Fri, 24 Apr 2020 14:24:49 GMT  
		Size: 3.7 MB (3720297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a608aeccf22dd87838d242b066fcfef55da359d339f2117793998950af90cb`  
		Last Modified: Fri, 24 Apr 2020 14:25:12 GMT  
		Size: 21.4 MB (21415464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4069f939d5ff89eccf4b1edaf61f16ee08f346689001f66c5406e5534c20d21f`  
		Last Modified: Fri, 24 Apr 2020 14:25:07 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:5a4e168ea396e61a8b853c77b239c34a52a3be61c7110311f567a373557fa0fe
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:9df10e6ff8b7ee79a0c0ad1c04cc4d85f0f91b7b0d67d8719169888d16eceebb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.9 MB (27909511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:955a6065421ce8267ab0aabea5e76ff6b00b60ea8bf3f76a6a77c7a08a213088`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:35 GMT
ADD file:a0afd0b0db7f9ee9496186ead087ec00edd1386ea8c018557d15720053f7308e in / 
# Fri, 24 Apr 2020 01:05:35 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 14:15:54 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 24 Apr 2020 14:24:06 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Fri, 24 Apr 2020 14:24:29 GMT
ENV TELEGRAF_VERSION=1.14.1
# Fri, 24 Apr 2020 14:24:33 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}-static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/telegraf.conf /etc/telegraf/ &&     chmod +x /usr/src/telegraf*/* &&     cp -a /usr/src/telegraf*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 24 Apr 2020 14:24:33 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 24 Apr 2020 14:24:34 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Fri, 24 Apr 2020 14:24:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 14:24:34 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:31603596830fc7e56753139f9c2c6bd3759e48a850659506ebfb885d1cf3aef5`  
		Last Modified: Fri, 24 Apr 2020 01:06:12 GMT  
		Size: 2.8 MB (2773413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321996f3080d1a7516b5914e27460b495eb04950d0190554844f395e7be9c793`  
		Last Modified: Fri, 24 Apr 2020 14:16:40 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21ceaab89b626cc487c744b86ea671176e8adf45ada4605d74c66278d136829`  
		Last Modified: Fri, 24 Apr 2020 14:24:49 GMT  
		Size: 3.7 MB (3720297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a608aeccf22dd87838d242b066fcfef55da359d339f2117793998950af90cb`  
		Last Modified: Fri, 24 Apr 2020 14:25:12 GMT  
		Size: 21.4 MB (21415464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4069f939d5ff89eccf4b1edaf61f16ee08f346689001f66c5406e5534c20d21f`  
		Last Modified: Fri, 24 Apr 2020 14:25:07 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:f6c959c3227f5b6521dc57e0355aa2d3256e39a191261e11588508ed3428f137
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:db9ddd787c33aed7a92cae7ff042c6a9609405e961e2589331df8899eac85a40
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.9 MB (97901818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d12ef0c09ccf5f26af0f760e9cb2531782bd5dafeee85c1854a4c1dc274e44c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 23 Apr 2020 00:22:48 GMT
ADD file:21bf6969c2166c361350c07b1089a1a4b34b7cd3e802a602385d83c49f44a7f6 in / 
# Thu, 23 Apr 2020 00:22:48 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 00:59:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 00:59:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 21:42:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 21:42:15 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Apr 2020 21:42:38 GMT
ENV TELEGRAF_VERSION=1.14.1
# Thu, 23 Apr 2020 21:42:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 23 Apr 2020 21:42:42 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 23 Apr 2020 21:42:42 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 23 Apr 2020 21:42:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 21:42:42 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:99760bc62448fbba69f6f0981d09bb4b7532e17362ecfb709141a7195d9b01d3`  
		Last Modified: Thu, 23 Apr 2020 00:27:35 GMT  
		Size: 45.4 MB (45375951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3fa264a7a881e244e7fd3420edda0d550ee3b26ed870f5c021d937497ffd602`  
		Last Modified: Thu, 23 Apr 2020 01:05:50 GMT  
		Size: 10.8 MB (10797279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a222a2af289fc1fe54c037f02e7651e0aead2f81f40cb2885786bfe57aed10a9`  
		Last Modified: Thu, 23 Apr 2020 01:05:48 GMT  
		Size: 4.3 MB (4340174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e55665c9e0e07356546d876ece60fc6716ce709a760ef15c81d71935f374ef3`  
		Last Modified: Thu, 23 Apr 2020 21:43:00 GMT  
		Size: 16.0 MB (15964715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b511841c00a1dc70b635eaba66db076226a14984974a828d6ea12e5e10138ced`  
		Last Modified: Thu, 23 Apr 2020 21:42:56 GMT  
		Size: 2.8 KB (2773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e412a1c29e41dd4673ebd026157db07b059b7a4fed6f8de3f8b530a21cbf00f`  
		Last Modified: Thu, 23 Apr 2020 21:43:20 GMT  
		Size: 21.4 MB (21420740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1067933cce2388d5b0bc901ab755d7be219d092463555fd857b681b30c3041`  
		Last Modified: Thu, 23 Apr 2020 21:43:16 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:a7dce1f73a4da00e5059a834d09b489f773418656e38dcf2b3024cde452e5841
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.5 MB (90490056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13d4e06057f2b37d4fb30349bd239d8e707a953144ee243986eacd6c0ebdf198`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 23 Apr 2020 01:07:13 GMT
ADD file:af00fcaffcce2a55b74d080d33cbc9ce5bcf91faf659b887f508c06803fa64bd in / 
# Thu, 23 Apr 2020 01:07:15 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 04:23:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 04:23:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 19:45:44 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 19:45:49 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Apr 2020 19:46:29 GMT
ENV TELEGRAF_VERSION=1.14.1
# Thu, 23 Apr 2020 19:46:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 23 Apr 2020 19:46:39 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 23 Apr 2020 19:46:40 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 23 Apr 2020 19:46:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 19:46:41 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4168e46f368afa15fa660f5197fb2946df81a85078c82e37a76d2610fb3999f1`  
		Last Modified: Thu, 23 Apr 2020 01:14:13 GMT  
		Size: 42.1 MB (42101192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9bc0e3bfcb00266e5034f08dae24b7862a41a069b0db0c68beb50e66983e602`  
		Last Modified: Thu, 23 Apr 2020 04:34:11 GMT  
		Size: 9.5 MB (9498287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3461f3bce5656c429f5d3faee144de5778a7f01ecd08241211c4badd34a7197b`  
		Last Modified: Thu, 23 Apr 2020 04:34:09 GMT  
		Size: 3.9 MB (3918722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c89366892b85101189243eb93a0a4a9fdbc21b615fc8d3aa603e1b2b6f1695c`  
		Last Modified: Thu, 23 Apr 2020 19:46:59 GMT  
		Size: 14.8 MB (14839164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74aa6be8071a1d0d4fcd5cda97ee3af0b63b759316ed4b27885d63e494e4958`  
		Last Modified: Thu, 23 Apr 2020 19:46:53 GMT  
		Size: 2.8 KB (2801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1668ff82c5768d9f7c77063b65d5396a641115f6052533b927c89becb2b030f3`  
		Last Modified: Thu, 23 Apr 2020 19:47:31 GMT  
		Size: 20.1 MB (20129704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3fde1a42a7bcfa704a405e3f4790ad507244e487583b74dff427d0d7be7f860`  
		Last Modified: Thu, 23 Apr 2020 19:47:23 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:e0e9994ef1393b3b18f01253cf333f7396a79eae0d0d36692d8a274bb656a9bd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.3 MB (92257106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c08609e65ef6813198e2378f60210aca502ec5d4b4b6242fd15d204cda6b465`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 23 Apr 2020 00:58:27 GMT
ADD file:4921b222c4914e830c4c018324aed1904bf1526e01493120ddc9c905373b2673 in / 
# Thu, 23 Apr 2020 00:58:29 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:46:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:46:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 23 Apr 2020 21:23:37 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 21:23:42 GMT
RUN set -ex &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Thu, 23 Apr 2020 21:24:15 GMT
ENV TELEGRAF_VERSION=1.14.1
# Thu, 23 Apr 2020 21:24:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 23 Apr 2020 21:24:21 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 23 Apr 2020 21:24:22 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 23 Apr 2020 21:24:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 23 Apr 2020 21:24:23 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:decabe2933bfe1939dff94ad523be4904c90e7bea69033943dd32f459d115bab`  
		Last Modified: Thu, 23 Apr 2020 01:05:29 GMT  
		Size: 43.2 MB (43159022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b030385917e3a4847f3280fab5601f7787447be0ac1b9ebdfc5a2b6f966d01`  
		Last Modified: Thu, 23 Apr 2020 03:55:16 GMT  
		Size: 9.7 MB (9748557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3766a78f146d565326c939891f33a75e49f3e5fb549c76d9d19ec413526bb4f0`  
		Last Modified: Thu, 23 Apr 2020 03:55:14 GMT  
		Size: 4.1 MB (4094419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e063050434db1728e621506c3cfad2c7c247fe84e03b3c33470cb1027d09a6`  
		Last Modified: Thu, 23 Apr 2020 21:24:40 GMT  
		Size: 15.5 MB (15530251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a6bf49b82384126f8c9969d6fd716c5ee05b38147cdd2abc4d6599541de512`  
		Last Modified: Thu, 23 Apr 2020 21:24:35 GMT  
		Size: 2.8 KB (2802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10dfa2bc79aad24602f2c690fbcb317d24f3b348e05e7982d21e1dde74c6a796`  
		Last Modified: Thu, 23 Apr 2020 21:25:08 GMT  
		Size: 19.7 MB (19721871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4feb40a14691c117e1ee7ac84afcad6c95c3e3ba24959792fb05adcbb68174e4`  
		Last Modified: Thu, 23 Apr 2020 21:25:02 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
