<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `telegraf`

-	[`telegraf:1.17`](#telegraf117)
-	[`telegraf:1.17-alpine`](#telegraf117-alpine)
-	[`telegraf:1.17.3`](#telegraf1173)
-	[`telegraf:1.17.3-alpine`](#telegraf1173-alpine)
-	[`telegraf:1.18`](#telegraf118)
-	[`telegraf:1.18-alpine`](#telegraf118-alpine)
-	[`telegraf:1.18.3`](#telegraf1183)
-	[`telegraf:1.18.3-alpine`](#telegraf1183-alpine)
-	[`telegraf:1.19`](#telegraf119)
-	[`telegraf:1.19-alpine`](#telegraf119-alpine)
-	[`telegraf:1.19.2`](#telegraf1192)
-	[`telegraf:1.19.2-alpine`](#telegraf1192-alpine)
-	[`telegraf:alpine`](#telegrafalpine)
-	[`telegraf:latest`](#telegraflatest)

## `telegraf:1.17`

```console
$ docker pull telegraf@sha256:8ad7278ffd55253f917ff2deaef69f9c28c5769eb2a375a0a8d0cd094a7510e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.17` - linux; amd64

```console
$ docker pull telegraf@sha256:8c3894f2192cd1c97ec581be0efbfc63faa9413b3acdbc36afeb70aa0313be22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.6 MB (108642884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1ca04abe3271aaed0c3159086a37e6560fabce4d371efa91dfef31f748895a6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 23 Jul 2021 02:31:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:31:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 23 Jul 2021 02:31:22 GMT
ENV TELEGRAF_VERSION=1.17.3
# Fri, 23 Jul 2021 02:31:25 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 23 Jul 2021 02:31:26 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 23 Jul 2021 02:31:26 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 23 Jul 2021 02:31:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 23 Jul 2021 02:31:26 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b36977b0126ab4ed0c6c426b7818fbdec01b96478c4726ecc075ab48b55af06`  
		Last Modified: Fri, 23 Jul 2021 02:32:20 GMT  
		Size: 17.4 MB (17415152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e54019056daf7d023e89716da7262cd724716a79043a07b501f6773d732b4e`  
		Last Modified: Fri, 23 Jul 2021 02:32:17 GMT  
		Size: 2.9 KB (2906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb4823cbb79e340baf1a3cae25736fd0a5cb0935bf0d58a36e13177fc7b8a26`  
		Last Modified: Fri, 23 Jul 2021 02:32:22 GMT  
		Size: 23.0 MB (22958848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0938e0cb221af5fc606aed4d113b5dff7585a27ca96f8031d7669da631189120`  
		Last Modified: Fri, 23 Jul 2021 02:32:17 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.17` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:c5860fe2455becc402548f89d4b8fb7def475bb063627c3f0714c68a15acfacf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.0 MB (100007429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c766625eb012a266c59412ccdda09981798e5ba4979dd8175c376ad8ee6d4bd8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:13 GMT
ADD file:c33137dc0d277fe210ea6387a8be105c625fdf777a541a6392896766df9919d4 in / 
# Thu, 22 Jul 2021 02:03:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:14:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:15:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 23 Jul 2021 11:03:25 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:03:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 23 Jul 2021 11:03:28 GMT
ENV TELEGRAF_VERSION=1.17.3
# Fri, 23 Jul 2021 11:03:36 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 23 Jul 2021 11:03:37 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 23 Jul 2021 11:03:37 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 23 Jul 2021 11:03:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 23 Jul 2021 11:03:38 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ff16e408fd8b8191145782047ebc0c76176550d844743a679143d53a164bea21`  
		Last Modified: Thu, 22 Jul 2021 02:15:33 GMT  
		Size: 45.9 MB (45917250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7701a3a4dc54422c371762f5416afea6835e02e9db10fd686f73159ec84ec2f7`  
		Last Modified: Thu, 22 Jul 2021 04:35:32 GMT  
		Size: 7.1 MB (7124233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8651c1854c791264fe60acc8ab39e9b914dc3258a9aa42509f1c35ce32a880d`  
		Last Modified: Thu, 22 Jul 2021 04:35:32 GMT  
		Size: 9.3 MB (9343793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2503b0beae04002464d92392e6fec2e284562e61a808159dca26a3b1fd759e35`  
		Last Modified: Fri, 23 Jul 2021 11:05:22 GMT  
		Size: 16.2 MB (16160458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc38ed3cb27fb443f2917c5bdc8189fa8831a0ae153b7c740183fc14c7c43ee`  
		Last Modified: Fri, 23 Jul 2021 11:05:10 GMT  
		Size: 2.9 KB (2892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f720d6112e52eb7365cbf8453d87a46e3e98004bcc794d96c912926a7a4fad`  
		Last Modified: Fri, 23 Jul 2021 11:05:23 GMT  
		Size: 21.5 MB (21458620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796df232203d33e3f3c324cfb32e7c8cf3067812781a03e9260e9fe7899dbfea`  
		Last Modified: Fri, 23 Jul 2021 11:05:10 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.17` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:8407a5e9c1db0fff62c39f5bbe03d08a7b6516ad870954a805d080a8b0e5a21b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105224737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a98673dcbfbbe3fd66e2ae2e5ee17dbf6d64762f3c96f6d53ece29cf3dacf380`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:59 GMT
ADD file:3e8e075f08a6b727602af05c539f43648a48663cbb3a88eeba310cfc32c01d78 in / 
# Thu, 22 Jul 2021 00:40:00 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:15:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:16:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 18:53:48 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 18:53:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 22 Jul 2021 18:53:51 GMT
ENV TELEGRAF_VERSION=1.17.3
# Thu, 22 Jul 2021 18:53:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 22 Jul 2021 18:53:55 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 22 Jul 2021 18:53:55 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 22 Jul 2021 18:53:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Jul 2021 18:53:55 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:d272b0d8f7c4fd0caf0ef022ce544cfe3800e349a73b585f82837e6526a4247e`  
		Last Modified: Thu, 22 Jul 2021 00:45:18 GMT  
		Size: 49.2 MB (49222109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fabd82f026fa10e0e0341fa3d6d3112de04413ea6c46e72bcc1dca40d924aa`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 7.7 MB (7694906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0193c0cdceae23cd0e13721651d74f409440171fe8a1c8b521616b6ed29db6e1`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 10.0 MB (9984335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec54281663350016ae8b6ed211f90d4f807346c559ef2e1fbeda84e1fa3055a6`  
		Last Modified: Thu, 22 Jul 2021 18:54:43 GMT  
		Size: 17.3 MB (17268593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cb5bf1c64ced1f6432366181164475b7a4cab1cd91f3237e3cf9b94140c7ba`  
		Last Modified: Thu, 22 Jul 2021 18:54:40 GMT  
		Size: 2.9 KB (2907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc849b9528dc2b3418c9a0bd51e9a679b73992369c1eb4dbbb14d278fe4d097`  
		Last Modified: Thu, 22 Jul 2021 18:54:44 GMT  
		Size: 21.1 MB (21051701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05ea9128760ff832d95247672f9453b8a7bf7b9c237e6dee159e81201e778e7`  
		Last Modified: Thu, 22 Jul 2021 18:54:40 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.17-alpine`

```console
$ docker pull telegraf@sha256:de4e4666bf07239391954b617792669d1b5ac822b2aafb312f96f9a9a7697682
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.17-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:f415febddaf18d090847627aa6f5135724f6343e4d7a60b58c09120d6ad107c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.9 MB (28922498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ff11c62bf60eaf0c868f0bd56cb731eaca38d6a2f366ebabcc221fdb23439f2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Apr 2021 02:35:34 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Thu, 15 Apr 2021 02:35:53 GMT
ENV TELEGRAF_VERSION=1.17.3
# Thu, 08 Jul 2021 00:20:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 08 Jul 2021 00:20:59 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 08 Jul 2021 00:20:59 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Thu, 08 Jul 2021 00:20:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Jul 2021 00:21:00 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661683aad4bf8006657c2bf1c3d74bfd343aaa18c1d5a30eda2d437ea8149e2e`  
		Last Modified: Thu, 15 Apr 2021 02:37:00 GMT  
		Size: 3.3 MB (3300674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd986e4a5f6c72f044b0dce6eaf1393bff8ecfdd4963e71fefa92c433b6f2ef6`  
		Last Modified: Thu, 08 Jul 2021 00:22:20 GMT  
		Size: 22.8 MB (22820920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df787a084ae1fb3873a20df3ecc7f2018ca361f58f844331a69110f8053cf0d9`  
		Last Modified: Thu, 08 Jul 2021 00:22:15 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.17.3`

```console
$ docker pull telegraf@sha256:8ad7278ffd55253f917ff2deaef69f9c28c5769eb2a375a0a8d0cd094a7510e6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.17.3` - linux; amd64

```console
$ docker pull telegraf@sha256:8c3894f2192cd1c97ec581be0efbfc63faa9413b3acdbc36afeb70aa0313be22
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.6 MB (108642884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1ca04abe3271aaed0c3159086a37e6560fabce4d371efa91dfef31f748895a6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 23 Jul 2021 02:31:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:31:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 23 Jul 2021 02:31:22 GMT
ENV TELEGRAF_VERSION=1.17.3
# Fri, 23 Jul 2021 02:31:25 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 23 Jul 2021 02:31:26 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 23 Jul 2021 02:31:26 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 23 Jul 2021 02:31:26 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 23 Jul 2021 02:31:26 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b36977b0126ab4ed0c6c426b7818fbdec01b96478c4726ecc075ab48b55af06`  
		Last Modified: Fri, 23 Jul 2021 02:32:20 GMT  
		Size: 17.4 MB (17415152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e54019056daf7d023e89716da7262cd724716a79043a07b501f6773d732b4e`  
		Last Modified: Fri, 23 Jul 2021 02:32:17 GMT  
		Size: 2.9 KB (2906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb4823cbb79e340baf1a3cae25736fd0a5cb0935bf0d58a36e13177fc7b8a26`  
		Last Modified: Fri, 23 Jul 2021 02:32:22 GMT  
		Size: 23.0 MB (22958848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0938e0cb221af5fc606aed4d113b5dff7585a27ca96f8031d7669da631189120`  
		Last Modified: Fri, 23 Jul 2021 02:32:17 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.17.3` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:c5860fe2455becc402548f89d4b8fb7def475bb063627c3f0714c68a15acfacf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.0 MB (100007429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c766625eb012a266c59412ccdda09981798e5ba4979dd8175c376ad8ee6d4bd8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:13 GMT
ADD file:c33137dc0d277fe210ea6387a8be105c625fdf777a541a6392896766df9919d4 in / 
# Thu, 22 Jul 2021 02:03:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:14:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:15:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 23 Jul 2021 11:03:25 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:03:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 23 Jul 2021 11:03:28 GMT
ENV TELEGRAF_VERSION=1.17.3
# Fri, 23 Jul 2021 11:03:36 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 23 Jul 2021 11:03:37 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 23 Jul 2021 11:03:37 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 23 Jul 2021 11:03:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 23 Jul 2021 11:03:38 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ff16e408fd8b8191145782047ebc0c76176550d844743a679143d53a164bea21`  
		Last Modified: Thu, 22 Jul 2021 02:15:33 GMT  
		Size: 45.9 MB (45917250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7701a3a4dc54422c371762f5416afea6835e02e9db10fd686f73159ec84ec2f7`  
		Last Modified: Thu, 22 Jul 2021 04:35:32 GMT  
		Size: 7.1 MB (7124233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8651c1854c791264fe60acc8ab39e9b914dc3258a9aa42509f1c35ce32a880d`  
		Last Modified: Thu, 22 Jul 2021 04:35:32 GMT  
		Size: 9.3 MB (9343793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2503b0beae04002464d92392e6fec2e284562e61a808159dca26a3b1fd759e35`  
		Last Modified: Fri, 23 Jul 2021 11:05:22 GMT  
		Size: 16.2 MB (16160458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc38ed3cb27fb443f2917c5bdc8189fa8831a0ae153b7c740183fc14c7c43ee`  
		Last Modified: Fri, 23 Jul 2021 11:05:10 GMT  
		Size: 2.9 KB (2892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f720d6112e52eb7365cbf8453d87a46e3e98004bcc794d96c912926a7a4fad`  
		Last Modified: Fri, 23 Jul 2021 11:05:23 GMT  
		Size: 21.5 MB (21458620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:796df232203d33e3f3c324cfb32e7c8cf3067812781a03e9260e9fe7899dbfea`  
		Last Modified: Fri, 23 Jul 2021 11:05:10 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.17.3` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:8407a5e9c1db0fff62c39f5bbe03d08a7b6516ad870954a805d080a8b0e5a21b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105224737 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a98673dcbfbbe3fd66e2ae2e5ee17dbf6d64762f3c96f6d53ece29cf3dacf380`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:59 GMT
ADD file:3e8e075f08a6b727602af05c539f43648a48663cbb3a88eeba310cfc32c01d78 in / 
# Thu, 22 Jul 2021 00:40:00 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:15:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:16:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 18:53:48 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 18:53:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 22 Jul 2021 18:53:51 GMT
ENV TELEGRAF_VERSION=1.17.3
# Thu, 22 Jul 2021 18:53:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 22 Jul 2021 18:53:55 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 22 Jul 2021 18:53:55 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 22 Jul 2021 18:53:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Jul 2021 18:53:55 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:d272b0d8f7c4fd0caf0ef022ce544cfe3800e349a73b585f82837e6526a4247e`  
		Last Modified: Thu, 22 Jul 2021 00:45:18 GMT  
		Size: 49.2 MB (49222109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fabd82f026fa10e0e0341fa3d6d3112de04413ea6c46e72bcc1dca40d924aa`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 7.7 MB (7694906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0193c0cdceae23cd0e13721651d74f409440171fe8a1c8b521616b6ed29db6e1`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 10.0 MB (9984335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec54281663350016ae8b6ed211f90d4f807346c559ef2e1fbeda84e1fa3055a6`  
		Last Modified: Thu, 22 Jul 2021 18:54:43 GMT  
		Size: 17.3 MB (17268593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cb5bf1c64ced1f6432366181164475b7a4cab1cd91f3237e3cf9b94140c7ba`  
		Last Modified: Thu, 22 Jul 2021 18:54:40 GMT  
		Size: 2.9 KB (2907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcc849b9528dc2b3418c9a0bd51e9a679b73992369c1eb4dbbb14d278fe4d097`  
		Last Modified: Thu, 22 Jul 2021 18:54:44 GMT  
		Size: 21.1 MB (21051701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c05ea9128760ff832d95247672f9453b8a7bf7b9c237e6dee159e81201e778e7`  
		Last Modified: Thu, 22 Jul 2021 18:54:40 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.17.3-alpine`

```console
$ docker pull telegraf@sha256:de4e4666bf07239391954b617792669d1b5ac822b2aafb312f96f9a9a7697682
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.17.3-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:f415febddaf18d090847627aa6f5135724f6343e4d7a60b58c09120d6ad107c0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.9 MB (28922498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ff11c62bf60eaf0c868f0bd56cb731eaca38d6a2f366ebabcc221fdb23439f2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Apr 2021 02:35:34 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Thu, 15 Apr 2021 02:35:53 GMT
ENV TELEGRAF_VERSION=1.17.3
# Thu, 08 Jul 2021 00:20:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 08 Jul 2021 00:20:59 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 08 Jul 2021 00:20:59 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Thu, 08 Jul 2021 00:20:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Jul 2021 00:21:00 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661683aad4bf8006657c2bf1c3d74bfd343aaa18c1d5a30eda2d437ea8149e2e`  
		Last Modified: Thu, 15 Apr 2021 02:37:00 GMT  
		Size: 3.3 MB (3300674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd986e4a5f6c72f044b0dce6eaf1393bff8ecfdd4963e71fefa92c433b6f2ef6`  
		Last Modified: Thu, 08 Jul 2021 00:22:20 GMT  
		Size: 22.8 MB (22820920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df787a084ae1fb3873a20df3ecc7f2018ca361f58f844331a69110f8053cf0d9`  
		Last Modified: Thu, 08 Jul 2021 00:22:15 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.18`

```console
$ docker pull telegraf@sha256:a84fda089d4d0592c6569062edafb8cec7b90fbee705d7eadf8221b69990fcb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.18` - linux; amd64

```console
$ docker pull telegraf@sha256:fea40c245d076573b5e304ed7dd378a7f249b24228f76a6fffb8a56735ea2165
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115491679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34535e6964f5053494b91e5c86328d4f67a73442653fdae10e9df5d5d9d69e3b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 23 Jul 2021 02:31:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:31:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 23 Jul 2021 02:31:32 GMT
ENV TELEGRAF_VERSION=1.18.3
# Fri, 23 Jul 2021 02:31:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 23 Jul 2021 02:31:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 23 Jul 2021 02:31:36 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 23 Jul 2021 02:31:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 23 Jul 2021 02:31:36 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b36977b0126ab4ed0c6c426b7818fbdec01b96478c4726ecc075ab48b55af06`  
		Last Modified: Fri, 23 Jul 2021 02:32:20 GMT  
		Size: 17.4 MB (17415152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e54019056daf7d023e89716da7262cd724716a79043a07b501f6773d732b4e`  
		Last Modified: Fri, 23 Jul 2021 02:32:17 GMT  
		Size: 2.9 KB (2906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53440cfbeb0ef29532448d0a3232d656f535f7423f8df0417d6ca955a7e7dc4`  
		Last Modified: Fri, 23 Jul 2021 02:32:41 GMT  
		Size: 29.8 MB (29807644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970d90a1686adc02baa21d6cb604a139536d42bc8899db319d85e366d89cacfe`  
		Last Modified: Fri, 23 Jul 2021 02:32:34 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.18` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:acbfd8e79d1d6615308e42ac3ef4983e42a31f3b29a01e605e92b1aff1c5dbcd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.1 MB (106103891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdb867bf7418ecf046fa5d9855810447fac37c71e1a60fda9fca1b365924cbae`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:13 GMT
ADD file:c33137dc0d277fe210ea6387a8be105c625fdf777a541a6392896766df9919d4 in / 
# Thu, 22 Jul 2021 02:03:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:14:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:15:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 23 Jul 2021 11:03:25 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:03:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 23 Jul 2021 11:03:49 GMT
ENV TELEGRAF_VERSION=1.18.3
# Fri, 23 Jul 2021 11:03:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 23 Jul 2021 11:03:59 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 23 Jul 2021 11:04:00 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 23 Jul 2021 11:04:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 23 Jul 2021 11:04:01 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ff16e408fd8b8191145782047ebc0c76176550d844743a679143d53a164bea21`  
		Last Modified: Thu, 22 Jul 2021 02:15:33 GMT  
		Size: 45.9 MB (45917250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7701a3a4dc54422c371762f5416afea6835e02e9db10fd686f73159ec84ec2f7`  
		Last Modified: Thu, 22 Jul 2021 04:35:32 GMT  
		Size: 7.1 MB (7124233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8651c1854c791264fe60acc8ab39e9b914dc3258a9aa42509f1c35ce32a880d`  
		Last Modified: Thu, 22 Jul 2021 04:35:32 GMT  
		Size: 9.3 MB (9343793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2503b0beae04002464d92392e6fec2e284562e61a808159dca26a3b1fd759e35`  
		Last Modified: Fri, 23 Jul 2021 11:05:22 GMT  
		Size: 16.2 MB (16160458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc38ed3cb27fb443f2917c5bdc8189fa8831a0ae153b7c740183fc14c7c43ee`  
		Last Modified: Fri, 23 Jul 2021 11:05:10 GMT  
		Size: 2.9 KB (2892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63dc2fc4578018f1f00f183b434e7a7046deae8c599b22c512d6581fa35808ce`  
		Last Modified: Fri, 23 Jul 2021 11:05:51 GMT  
		Size: 27.6 MB (27555080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0618c1df540d7e37ac54a1708f268140efb6be43307760a8e09a6cdec81a0e8e`  
		Last Modified: Fri, 23 Jul 2021 11:05:34 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.18` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:83dc86bad39d066acec6bd8089c71a6ea11d7dd648f3dcc7a987deb74bf000d1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.1 MB (111146756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee2ac04f3e53c8ec9e63c0331f7d7e6ae46507f144dd4071448da77087ee4b73`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:59 GMT
ADD file:3e8e075f08a6b727602af05c539f43648a48663cbb3a88eeba310cfc32c01d78 in / 
# Thu, 22 Jul 2021 00:40:00 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:15:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:16:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 18:53:48 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 18:53:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 22 Jul 2021 18:54:01 GMT
ENV TELEGRAF_VERSION=1.18.3
# Thu, 22 Jul 2021 18:54:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 22 Jul 2021 18:54:05 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 22 Jul 2021 18:54:06 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 22 Jul 2021 18:54:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Jul 2021 18:54:06 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:d272b0d8f7c4fd0caf0ef022ce544cfe3800e349a73b585f82837e6526a4247e`  
		Last Modified: Thu, 22 Jul 2021 00:45:18 GMT  
		Size: 49.2 MB (49222109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fabd82f026fa10e0e0341fa3d6d3112de04413ea6c46e72bcc1dca40d924aa`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 7.7 MB (7694906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0193c0cdceae23cd0e13721651d74f409440171fe8a1c8b521616b6ed29db6e1`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 10.0 MB (9984335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec54281663350016ae8b6ed211f90d4f807346c559ef2e1fbeda84e1fa3055a6`  
		Last Modified: Thu, 22 Jul 2021 18:54:43 GMT  
		Size: 17.3 MB (17268593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cb5bf1c64ced1f6432366181164475b7a4cab1cd91f3237e3cf9b94140c7ba`  
		Last Modified: Thu, 22 Jul 2021 18:54:40 GMT  
		Size: 2.9 KB (2907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c54c8e256e2e45e8609d946af2048d0b4b9677e4d42cf9dd8bbfa95a5b6867`  
		Last Modified: Thu, 22 Jul 2021 18:55:03 GMT  
		Size: 27.0 MB (26973723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49e430bcb76fe7fc497cd34b0b8cb3851d888aa0ede72af8ac1cb4b7db48d28`  
		Last Modified: Thu, 22 Jul 2021 18:54:56 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.18-alpine`

```console
$ docker pull telegraf@sha256:f0b185ac5a9704cf1c235093175707a3d88e60292930d5c030380ebcea8966f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.18-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:ad514b1959d4331e83c1ab1d7407eecb24168750783c875a300ba6f6b0cacbdd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.8 MB (35763257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e28459c5b4cb2457ff58e37c287cfe685a6fdd2428eb4ab04caa52c6b0a16eab`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Apr 2021 02:35:34 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Mon, 24 May 2021 19:45:54 GMT
ENV TELEGRAF_VERSION=1.18.3
# Thu, 08 Jul 2021 00:21:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 08 Jul 2021 00:21:19 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 08 Jul 2021 00:21:19 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Thu, 08 Jul 2021 00:21:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Jul 2021 00:21:20 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661683aad4bf8006657c2bf1c3d74bfd343aaa18c1d5a30eda2d437ea8149e2e`  
		Last Modified: Thu, 15 Apr 2021 02:37:00 GMT  
		Size: 3.3 MB (3300674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b62d4a69768d9012f90e50e0ff93d8537ea4c0baf89c6893fa070c649d2a3b2`  
		Last Modified: Thu, 08 Jul 2021 00:22:52 GMT  
		Size: 29.7 MB (29661678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2784e71fb1eaf7c6db2734f38457c04e82376a74708585c3861cbe6d247805d2`  
		Last Modified: Thu, 08 Jul 2021 00:22:46 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.18.3`

```console
$ docker pull telegraf@sha256:a84fda089d4d0592c6569062edafb8cec7b90fbee705d7eadf8221b69990fcb0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.18.3` - linux; amd64

```console
$ docker pull telegraf@sha256:fea40c245d076573b5e304ed7dd378a7f249b24228f76a6fffb8a56735ea2165
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115491679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34535e6964f5053494b91e5c86328d4f67a73442653fdae10e9df5d5d9d69e3b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 23 Jul 2021 02:31:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:31:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 23 Jul 2021 02:31:32 GMT
ENV TELEGRAF_VERSION=1.18.3
# Fri, 23 Jul 2021 02:31:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 23 Jul 2021 02:31:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 23 Jul 2021 02:31:36 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 23 Jul 2021 02:31:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 23 Jul 2021 02:31:36 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b36977b0126ab4ed0c6c426b7818fbdec01b96478c4726ecc075ab48b55af06`  
		Last Modified: Fri, 23 Jul 2021 02:32:20 GMT  
		Size: 17.4 MB (17415152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e54019056daf7d023e89716da7262cd724716a79043a07b501f6773d732b4e`  
		Last Modified: Fri, 23 Jul 2021 02:32:17 GMT  
		Size: 2.9 KB (2906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53440cfbeb0ef29532448d0a3232d656f535f7423f8df0417d6ca955a7e7dc4`  
		Last Modified: Fri, 23 Jul 2021 02:32:41 GMT  
		Size: 29.8 MB (29807644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970d90a1686adc02baa21d6cb604a139536d42bc8899db319d85e366d89cacfe`  
		Last Modified: Fri, 23 Jul 2021 02:32:34 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.18.3` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:acbfd8e79d1d6615308e42ac3ef4983e42a31f3b29a01e605e92b1aff1c5dbcd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.1 MB (106103891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdb867bf7418ecf046fa5d9855810447fac37c71e1a60fda9fca1b365924cbae`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:13 GMT
ADD file:c33137dc0d277fe210ea6387a8be105c625fdf777a541a6392896766df9919d4 in / 
# Thu, 22 Jul 2021 02:03:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:14:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:15:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 23 Jul 2021 11:03:25 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:03:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 23 Jul 2021 11:03:49 GMT
ENV TELEGRAF_VERSION=1.18.3
# Fri, 23 Jul 2021 11:03:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 23 Jul 2021 11:03:59 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 23 Jul 2021 11:04:00 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 23 Jul 2021 11:04:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 23 Jul 2021 11:04:01 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ff16e408fd8b8191145782047ebc0c76176550d844743a679143d53a164bea21`  
		Last Modified: Thu, 22 Jul 2021 02:15:33 GMT  
		Size: 45.9 MB (45917250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7701a3a4dc54422c371762f5416afea6835e02e9db10fd686f73159ec84ec2f7`  
		Last Modified: Thu, 22 Jul 2021 04:35:32 GMT  
		Size: 7.1 MB (7124233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8651c1854c791264fe60acc8ab39e9b914dc3258a9aa42509f1c35ce32a880d`  
		Last Modified: Thu, 22 Jul 2021 04:35:32 GMT  
		Size: 9.3 MB (9343793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2503b0beae04002464d92392e6fec2e284562e61a808159dca26a3b1fd759e35`  
		Last Modified: Fri, 23 Jul 2021 11:05:22 GMT  
		Size: 16.2 MB (16160458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc38ed3cb27fb443f2917c5bdc8189fa8831a0ae153b7c740183fc14c7c43ee`  
		Last Modified: Fri, 23 Jul 2021 11:05:10 GMT  
		Size: 2.9 KB (2892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63dc2fc4578018f1f00f183b434e7a7046deae8c599b22c512d6581fa35808ce`  
		Last Modified: Fri, 23 Jul 2021 11:05:51 GMT  
		Size: 27.6 MB (27555080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0618c1df540d7e37ac54a1708f268140efb6be43307760a8e09a6cdec81a0e8e`  
		Last Modified: Fri, 23 Jul 2021 11:05:34 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.18.3` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:83dc86bad39d066acec6bd8089c71a6ea11d7dd648f3dcc7a987deb74bf000d1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.1 MB (111146756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee2ac04f3e53c8ec9e63c0331f7d7e6ae46507f144dd4071448da77087ee4b73`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:59 GMT
ADD file:3e8e075f08a6b727602af05c539f43648a48663cbb3a88eeba310cfc32c01d78 in / 
# Thu, 22 Jul 2021 00:40:00 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:15:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:16:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 18:53:48 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 18:53:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 22 Jul 2021 18:54:01 GMT
ENV TELEGRAF_VERSION=1.18.3
# Thu, 22 Jul 2021 18:54:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 22 Jul 2021 18:54:05 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 22 Jul 2021 18:54:06 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 22 Jul 2021 18:54:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Jul 2021 18:54:06 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:d272b0d8f7c4fd0caf0ef022ce544cfe3800e349a73b585f82837e6526a4247e`  
		Last Modified: Thu, 22 Jul 2021 00:45:18 GMT  
		Size: 49.2 MB (49222109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fabd82f026fa10e0e0341fa3d6d3112de04413ea6c46e72bcc1dca40d924aa`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 7.7 MB (7694906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0193c0cdceae23cd0e13721651d74f409440171fe8a1c8b521616b6ed29db6e1`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 10.0 MB (9984335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec54281663350016ae8b6ed211f90d4f807346c559ef2e1fbeda84e1fa3055a6`  
		Last Modified: Thu, 22 Jul 2021 18:54:43 GMT  
		Size: 17.3 MB (17268593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cb5bf1c64ced1f6432366181164475b7a4cab1cd91f3237e3cf9b94140c7ba`  
		Last Modified: Thu, 22 Jul 2021 18:54:40 GMT  
		Size: 2.9 KB (2907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c54c8e256e2e45e8609d946af2048d0b4b9677e4d42cf9dd8bbfa95a5b6867`  
		Last Modified: Thu, 22 Jul 2021 18:55:03 GMT  
		Size: 27.0 MB (26973723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49e430bcb76fe7fc497cd34b0b8cb3851d888aa0ede72af8ac1cb4b7db48d28`  
		Last Modified: Thu, 22 Jul 2021 18:54:56 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.18.3-alpine`

```console
$ docker pull telegraf@sha256:f0b185ac5a9704cf1c235093175707a3d88e60292930d5c030380ebcea8966f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.18.3-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:ad514b1959d4331e83c1ab1d7407eecb24168750783c875a300ba6f6b0cacbdd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.8 MB (35763257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e28459c5b4cb2457ff58e37c287cfe685a6fdd2428eb4ab04caa52c6b0a16eab`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Apr 2021 02:35:34 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Mon, 24 May 2021 19:45:54 GMT
ENV TELEGRAF_VERSION=1.18.3
# Thu, 08 Jul 2021 00:21:19 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 08 Jul 2021 00:21:19 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 08 Jul 2021 00:21:19 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Thu, 08 Jul 2021 00:21:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Jul 2021 00:21:20 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661683aad4bf8006657c2bf1c3d74bfd343aaa18c1d5a30eda2d437ea8149e2e`  
		Last Modified: Thu, 15 Apr 2021 02:37:00 GMT  
		Size: 3.3 MB (3300674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b62d4a69768d9012f90e50e0ff93d8537ea4c0baf89c6893fa070c649d2a3b2`  
		Last Modified: Thu, 08 Jul 2021 00:22:52 GMT  
		Size: 29.7 MB (29661678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2784e71fb1eaf7c6db2734f38457c04e82376a74708585c3861cbe6d247805d2`  
		Last Modified: Thu, 08 Jul 2021 00:22:46 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.19`

```console
$ docker pull telegraf@sha256:e2a7895d58f111407bc00d81e9c0861567d1d41fb125f0c36edd8ec6b621d9d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.19` - linux; amd64

```console
$ docker pull telegraf@sha256:8b476a4ade2c139a50d9e5ede075b779bb50a5f0e424ee3336a21533267c503b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118759622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93c1c818d6e1d3a558f20fad414ebdb1b901d7338e013623cd6b78dad80a1d85`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 23 Jul 2021 02:31:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:31:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 23 Jul 2021 02:31:44 GMT
ENV TELEGRAF_VERSION=1.19.1
# Fri, 23 Jul 2021 02:31:49 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 23 Jul 2021 02:31:49 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 23 Jul 2021 02:31:50 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 23 Jul 2021 02:31:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 23 Jul 2021 02:31:50 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b36977b0126ab4ed0c6c426b7818fbdec01b96478c4726ecc075ab48b55af06`  
		Last Modified: Fri, 23 Jul 2021 02:32:20 GMT  
		Size: 17.4 MB (17415152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e54019056daf7d023e89716da7262cd724716a79043a07b501f6773d732b4e`  
		Last Modified: Fri, 23 Jul 2021 02:32:17 GMT  
		Size: 2.9 KB (2906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28990859d49c4fbfb50639d788992c510d37a577e56082d1bb683ec20af04dcf`  
		Last Modified: Fri, 23 Jul 2021 02:33:02 GMT  
		Size: 33.1 MB (33075587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e74ce2de5a89b9f6d83343737e0ba43555c68a5a5cee0f485c378651dea5fb0`  
		Last Modified: Fri, 23 Jul 2021 02:32:53 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.19` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:62ff41061b6321337e883b8e4f42d6709a44820e62130291b15dac131b77990c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110131231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d59ecacc78142a6cf4d81df0466ac8b3fc4a04d30b3f25fafd37e2cbcd43bee2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:13 GMT
ADD file:c33137dc0d277fe210ea6387a8be105c625fdf777a541a6392896766df9919d4 in / 
# Thu, 22 Jul 2021 02:03:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:14:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:15:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 23 Jul 2021 11:03:25 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:03:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 29 Jul 2021 23:51:17 GMT
ENV TELEGRAF_VERSION=1.19.2
# Thu, 29 Jul 2021 23:51:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 29 Jul 2021 23:51:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 29 Jul 2021 23:51:30 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 29 Jul 2021 23:51:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 29 Jul 2021 23:51:30 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ff16e408fd8b8191145782047ebc0c76176550d844743a679143d53a164bea21`  
		Last Modified: Thu, 22 Jul 2021 02:15:33 GMT  
		Size: 45.9 MB (45917250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7701a3a4dc54422c371762f5416afea6835e02e9db10fd686f73159ec84ec2f7`  
		Last Modified: Thu, 22 Jul 2021 04:35:32 GMT  
		Size: 7.1 MB (7124233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8651c1854c791264fe60acc8ab39e9b914dc3258a9aa42509f1c35ce32a880d`  
		Last Modified: Thu, 22 Jul 2021 04:35:32 GMT  
		Size: 9.3 MB (9343793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2503b0beae04002464d92392e6fec2e284562e61a808159dca26a3b1fd759e35`  
		Last Modified: Fri, 23 Jul 2021 11:05:22 GMT  
		Size: 16.2 MB (16160458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc38ed3cb27fb443f2917c5bdc8189fa8831a0ae153b7c740183fc14c7c43ee`  
		Last Modified: Fri, 23 Jul 2021 11:05:10 GMT  
		Size: 2.9 KB (2892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904212545166c39935a87d5761d96757d92fc88956b16a3d2fe01989ff473799`  
		Last Modified: Thu, 29 Jul 2021 23:52:42 GMT  
		Size: 31.6 MB (31582420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84adccc3c7b8c3c1c6d00a502eed47b0fdc0ab12af045f044c9df3ac0e3f1ae`  
		Last Modified: Thu, 29 Jul 2021 23:52:19 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.19` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:47d833e21b4c0f4165595359fd7afb08e323cc21d8153ef055001db544f8f239
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.0 MB (115031423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94dd3b8c501cab2122522d1c951d3ee460f0e2e98f873be96e945a4599c198fb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:59 GMT
ADD file:3e8e075f08a6b727602af05c539f43648a48663cbb3a88eeba310cfc32c01d78 in / 
# Thu, 22 Jul 2021 00:40:00 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:15:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:16:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 18:53:48 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 18:53:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 29 Jul 2021 22:41:03 GMT
ENV TELEGRAF_VERSION=1.19.2
# Thu, 29 Jul 2021 22:41:12 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 29 Jul 2021 22:41:12 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 29 Jul 2021 22:41:13 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 29 Jul 2021 22:41:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 29 Jul 2021 22:41:13 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:d272b0d8f7c4fd0caf0ef022ce544cfe3800e349a73b585f82837e6526a4247e`  
		Last Modified: Thu, 22 Jul 2021 00:45:18 GMT  
		Size: 49.2 MB (49222109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fabd82f026fa10e0e0341fa3d6d3112de04413ea6c46e72bcc1dca40d924aa`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 7.7 MB (7694906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0193c0cdceae23cd0e13721651d74f409440171fe8a1c8b521616b6ed29db6e1`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 10.0 MB (9984335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec54281663350016ae8b6ed211f90d4f807346c559ef2e1fbeda84e1fa3055a6`  
		Last Modified: Thu, 22 Jul 2021 18:54:43 GMT  
		Size: 17.3 MB (17268593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cb5bf1c64ced1f6432366181164475b7a4cab1cd91f3237e3cf9b94140c7ba`  
		Last Modified: Thu, 22 Jul 2021 18:54:40 GMT  
		Size: 2.9 KB (2907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21958e949fe444025a3b939600a455bfbe159650a30d30453c2ef0abe2f35f16`  
		Last Modified: Thu, 29 Jul 2021 22:41:44 GMT  
		Size: 30.9 MB (30858388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ced1971d75484ac5e31cb6e2aaae4e3b9071326f360f13efb35d5e127646916`  
		Last Modified: Thu, 29 Jul 2021 22:41:38 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.19-alpine`

```console
$ docker pull telegraf@sha256:2933b7dd72888ef72e3c4bfc8ee540b929dd5371e5a7636c157d3a5d3422bd24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.19-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:9159740897e09905277d41e5dabe92f4f14d44a6d1eae0687e0a339d73f57d0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (39023457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d38b66159696edd123212a7d841a161205e68e77341c05c9d119c9dc51ef01a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Apr 2021 02:35:34 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Thu, 08 Jul 2021 00:21:33 GMT
ENV TELEGRAF_VERSION=1.19.1
# Thu, 08 Jul 2021 00:21:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 08 Jul 2021 00:21:38 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 08 Jul 2021 00:21:38 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Thu, 08 Jul 2021 00:21:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Jul 2021 00:21:38 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661683aad4bf8006657c2bf1c3d74bfd343aaa18c1d5a30eda2d437ea8149e2e`  
		Last Modified: Thu, 15 Apr 2021 02:37:00 GMT  
		Size: 3.3 MB (3300674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a772266ecd71bd9d10a18bc7fbc8c872fd1f1d35c4aeda56a6afa564c9fdf3`  
		Last Modified: Thu, 08 Jul 2021 00:23:29 GMT  
		Size: 32.9 MB (32921879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6878432d8c1d3e8a77786eee661b1fdada1b4c2c2b696b18f867597ffebd756a`  
		Last Modified: Thu, 08 Jul 2021 00:23:23 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.19.2`

```console
$ docker pull telegraf@sha256:e1b809669cd6614cc926d622234999c100b6b2b6093b306a071619e4613cda56
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.19.2` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:62ff41061b6321337e883b8e4f42d6709a44820e62130291b15dac131b77990c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110131231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d59ecacc78142a6cf4d81df0466ac8b3fc4a04d30b3f25fafd37e2cbcd43bee2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:13 GMT
ADD file:c33137dc0d277fe210ea6387a8be105c625fdf777a541a6392896766df9919d4 in / 
# Thu, 22 Jul 2021 02:03:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:14:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:15:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 23 Jul 2021 11:03:25 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:03:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 29 Jul 2021 23:51:17 GMT
ENV TELEGRAF_VERSION=1.19.2
# Thu, 29 Jul 2021 23:51:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 29 Jul 2021 23:51:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 29 Jul 2021 23:51:30 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 29 Jul 2021 23:51:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 29 Jul 2021 23:51:30 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ff16e408fd8b8191145782047ebc0c76176550d844743a679143d53a164bea21`  
		Last Modified: Thu, 22 Jul 2021 02:15:33 GMT  
		Size: 45.9 MB (45917250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7701a3a4dc54422c371762f5416afea6835e02e9db10fd686f73159ec84ec2f7`  
		Last Modified: Thu, 22 Jul 2021 04:35:32 GMT  
		Size: 7.1 MB (7124233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8651c1854c791264fe60acc8ab39e9b914dc3258a9aa42509f1c35ce32a880d`  
		Last Modified: Thu, 22 Jul 2021 04:35:32 GMT  
		Size: 9.3 MB (9343793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2503b0beae04002464d92392e6fec2e284562e61a808159dca26a3b1fd759e35`  
		Last Modified: Fri, 23 Jul 2021 11:05:22 GMT  
		Size: 16.2 MB (16160458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc38ed3cb27fb443f2917c5bdc8189fa8831a0ae153b7c740183fc14c7c43ee`  
		Last Modified: Fri, 23 Jul 2021 11:05:10 GMT  
		Size: 2.9 KB (2892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904212545166c39935a87d5761d96757d92fc88956b16a3d2fe01989ff473799`  
		Last Modified: Thu, 29 Jul 2021 23:52:42 GMT  
		Size: 31.6 MB (31582420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84adccc3c7b8c3c1c6d00a502eed47b0fdc0ab12af045f044c9df3ac0e3f1ae`  
		Last Modified: Thu, 29 Jul 2021 23:52:19 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.19.2` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:47d833e21b4c0f4165595359fd7afb08e323cc21d8153ef055001db544f8f239
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.0 MB (115031423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94dd3b8c501cab2122522d1c951d3ee460f0e2e98f873be96e945a4599c198fb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:59 GMT
ADD file:3e8e075f08a6b727602af05c539f43648a48663cbb3a88eeba310cfc32c01d78 in / 
# Thu, 22 Jul 2021 00:40:00 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:15:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:16:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 18:53:48 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 18:53:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 29 Jul 2021 22:41:03 GMT
ENV TELEGRAF_VERSION=1.19.2
# Thu, 29 Jul 2021 22:41:12 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 29 Jul 2021 22:41:12 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 29 Jul 2021 22:41:13 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 29 Jul 2021 22:41:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 29 Jul 2021 22:41:13 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:d272b0d8f7c4fd0caf0ef022ce544cfe3800e349a73b585f82837e6526a4247e`  
		Last Modified: Thu, 22 Jul 2021 00:45:18 GMT  
		Size: 49.2 MB (49222109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fabd82f026fa10e0e0341fa3d6d3112de04413ea6c46e72bcc1dca40d924aa`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 7.7 MB (7694906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0193c0cdceae23cd0e13721651d74f409440171fe8a1c8b521616b6ed29db6e1`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 10.0 MB (9984335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec54281663350016ae8b6ed211f90d4f807346c559ef2e1fbeda84e1fa3055a6`  
		Last Modified: Thu, 22 Jul 2021 18:54:43 GMT  
		Size: 17.3 MB (17268593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cb5bf1c64ced1f6432366181164475b7a4cab1cd91f3237e3cf9b94140c7ba`  
		Last Modified: Thu, 22 Jul 2021 18:54:40 GMT  
		Size: 2.9 KB (2907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21958e949fe444025a3b939600a455bfbe159650a30d30453c2ef0abe2f35f16`  
		Last Modified: Thu, 29 Jul 2021 22:41:44 GMT  
		Size: 30.9 MB (30858388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ced1971d75484ac5e31cb6e2aaae4e3b9071326f360f13efb35d5e127646916`  
		Last Modified: Thu, 29 Jul 2021 22:41:38 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.19.2-alpine`

```console
$ docker pull telegraf@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:2933b7dd72888ef72e3c4bfc8ee540b929dd5371e5a7636c157d3a5d3422bd24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:9159740897e09905277d41e5dabe92f4f14d44a6d1eae0687e0a339d73f57d0b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.0 MB (39023457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d38b66159696edd123212a7d841a161205e68e77341c05c9d119c9dc51ef01a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Apr 2021 02:35:34 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Thu, 08 Jul 2021 00:21:33 GMT
ENV TELEGRAF_VERSION=1.19.1
# Thu, 08 Jul 2021 00:21:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 08 Jul 2021 00:21:38 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 08 Jul 2021 00:21:38 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Thu, 08 Jul 2021 00:21:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Jul 2021 00:21:38 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661683aad4bf8006657c2bf1c3d74bfd343aaa18c1d5a30eda2d437ea8149e2e`  
		Last Modified: Thu, 15 Apr 2021 02:37:00 GMT  
		Size: 3.3 MB (3300674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a772266ecd71bd9d10a18bc7fbc8c872fd1f1d35c4aeda56a6afa564c9fdf3`  
		Last Modified: Thu, 08 Jul 2021 00:23:29 GMT  
		Size: 32.9 MB (32921879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6878432d8c1d3e8a77786eee661b1fdada1b4c2c2b696b18f867597ffebd756a`  
		Last Modified: Thu, 08 Jul 2021 00:23:23 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:e2a7895d58f111407bc00d81e9c0861567d1d41fb125f0c36edd8ec6b621d9d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:8b476a4ade2c139a50d9e5ede075b779bb50a5f0e424ee3336a21533267c503b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118759622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93c1c818d6e1d3a558f20fad414ebdb1b901d7338e013623cd6b78dad80a1d85`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 22 Jul 2021 00:45:30 GMT
ADD file:e952f6979e4b0ead00b6906db1dd70eb9beb564a04e2f02e2e0cff8614920216 in / 
# Thu, 22 Jul 2021 00:45:31 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:12:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:12:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 23 Jul 2021 02:31:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 02:31:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 23 Jul 2021 02:31:44 GMT
ENV TELEGRAF_VERSION=1.19.1
# Fri, 23 Jul 2021 02:31:49 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 23 Jul 2021 02:31:49 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 23 Jul 2021 02:31:50 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 23 Jul 2021 02:31:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 23 Jul 2021 02:31:50 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:627b765e08d177e63c9a202ca4991b711448905b934435c70b7cbd7d4a9c7959`  
		Last Modified: Thu, 22 Jul 2021 00:50:07 GMT  
		Size: 50.4 MB (50435626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c040670e5e559fd936db175530ad4c1dd014bd25b2bf25ea19fa20554fe2d736`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 7.8 MB (7832944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a180f4992853fa3dd8da604e7b041bc8ea92157749d042c0853312f178f6a`  
		Last Modified: Thu, 22 Jul 2021 01:19:54 GMT  
		Size: 10.0 MB (9997222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b36977b0126ab4ed0c6c426b7818fbdec01b96478c4726ecc075ab48b55af06`  
		Last Modified: Fri, 23 Jul 2021 02:32:20 GMT  
		Size: 17.4 MB (17415152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e54019056daf7d023e89716da7262cd724716a79043a07b501f6773d732b4e`  
		Last Modified: Fri, 23 Jul 2021 02:32:17 GMT  
		Size: 2.9 KB (2906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28990859d49c4fbfb50639d788992c510d37a577e56082d1bb683ec20af04dcf`  
		Last Modified: Fri, 23 Jul 2021 02:33:02 GMT  
		Size: 33.1 MB (33075587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e74ce2de5a89b9f6d83343737e0ba43555c68a5a5cee0f485c378651dea5fb0`  
		Last Modified: Fri, 23 Jul 2021 02:32:53 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:62ff41061b6321337e883b8e4f42d6709a44820e62130291b15dac131b77990c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110131231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d59ecacc78142a6cf4d81df0466ac8b3fc4a04d30b3f25fafd37e2cbcd43bee2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 22 Jul 2021 02:03:13 GMT
ADD file:c33137dc0d277fe210ea6387a8be105c625fdf777a541a6392896766df9919d4 in / 
# Thu, 22 Jul 2021 02:03:14 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 04:14:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 04:15:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 23 Jul 2021 11:03:25 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Fri, 23 Jul 2021 11:03:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 29 Jul 2021 23:51:17 GMT
ENV TELEGRAF_VERSION=1.19.2
# Thu, 29 Jul 2021 23:51:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 29 Jul 2021 23:51:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 29 Jul 2021 23:51:30 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 29 Jul 2021 23:51:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 29 Jul 2021 23:51:30 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ff16e408fd8b8191145782047ebc0c76176550d844743a679143d53a164bea21`  
		Last Modified: Thu, 22 Jul 2021 02:15:33 GMT  
		Size: 45.9 MB (45917250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7701a3a4dc54422c371762f5416afea6835e02e9db10fd686f73159ec84ec2f7`  
		Last Modified: Thu, 22 Jul 2021 04:35:32 GMT  
		Size: 7.1 MB (7124233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8651c1854c791264fe60acc8ab39e9b914dc3258a9aa42509f1c35ce32a880d`  
		Last Modified: Thu, 22 Jul 2021 04:35:32 GMT  
		Size: 9.3 MB (9343793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2503b0beae04002464d92392e6fec2e284562e61a808159dca26a3b1fd759e35`  
		Last Modified: Fri, 23 Jul 2021 11:05:22 GMT  
		Size: 16.2 MB (16160458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc38ed3cb27fb443f2917c5bdc8189fa8831a0ae153b7c740183fc14c7c43ee`  
		Last Modified: Fri, 23 Jul 2021 11:05:10 GMT  
		Size: 2.9 KB (2892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:904212545166c39935a87d5761d96757d92fc88956b16a3d2fe01989ff473799`  
		Last Modified: Thu, 29 Jul 2021 23:52:42 GMT  
		Size: 31.6 MB (31582420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84adccc3c7b8c3c1c6d00a502eed47b0fdc0ab12af045f044c9df3ac0e3f1ae`  
		Last Modified: Thu, 29 Jul 2021 23:52:19 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:47d833e21b4c0f4165595359fd7afb08e323cc21d8153ef055001db544f8f239
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.0 MB (115031423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94dd3b8c501cab2122522d1c951d3ee460f0e2e98f873be96e945a4599c198fb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 22 Jul 2021 00:39:59 GMT
ADD file:3e8e075f08a6b727602af05c539f43648a48663cbb3a88eeba310cfc32c01d78 in / 
# Thu, 22 Jul 2021 00:40:00 GMT
CMD ["bash"]
# Thu, 22 Jul 2021 01:15:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 01:16:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 22 Jul 2021 18:53:48 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Thu, 22 Jul 2021 18:53:50 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 29 Jul 2021 22:41:03 GMT
ENV TELEGRAF_VERSION=1.19.2
# Thu, 29 Jul 2021 22:41:12 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 29 Jul 2021 22:41:12 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 29 Jul 2021 22:41:13 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Thu, 29 Jul 2021 22:41:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 29 Jul 2021 22:41:13 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:d272b0d8f7c4fd0caf0ef022ce544cfe3800e349a73b585f82837e6526a4247e`  
		Last Modified: Thu, 22 Jul 2021 00:45:18 GMT  
		Size: 49.2 MB (49222109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fabd82f026fa10e0e0341fa3d6d3112de04413ea6c46e72bcc1dca40d924aa`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 7.7 MB (7694906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0193c0cdceae23cd0e13721651d74f409440171fe8a1c8b521616b6ed29db6e1`  
		Last Modified: Thu, 22 Jul 2021 01:25:00 GMT  
		Size: 10.0 MB (9984335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec54281663350016ae8b6ed211f90d4f807346c559ef2e1fbeda84e1fa3055a6`  
		Last Modified: Thu, 22 Jul 2021 18:54:43 GMT  
		Size: 17.3 MB (17268593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cb5bf1c64ced1f6432366181164475b7a4cab1cd91f3237e3cf9b94140c7ba`  
		Last Modified: Thu, 22 Jul 2021 18:54:40 GMT  
		Size: 2.9 KB (2907 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21958e949fe444025a3b939600a455bfbe159650a30d30453c2ef0abe2f35f16`  
		Last Modified: Thu, 29 Jul 2021 22:41:44 GMT  
		Size: 30.9 MB (30858388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ced1971d75484ac5e31cb6e2aaae4e3b9071326f360f13efb35d5e127646916`  
		Last Modified: Thu, 29 Jul 2021 22:41:38 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
