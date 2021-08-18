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
$ docker pull telegraf@sha256:5d3090b5e4d8744d3f5013ba20bb756a4ddd039b0f4d029984659d8eb7423936
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
$ docker pull telegraf@sha256:3787fc1730c5cf84b2c9098a086ecc2ffcd943e2b9821e67f74960b7a326426f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105225274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2030074ffd2bf35bcff436742fff780f1ad2be6ab1b46298638951704cd515dc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:16 GMT
ADD file:9e7d801ba29c50f7388cf80395faef75e0b4db056e16d1117293539bda895467 in / 
# Tue, 17 Aug 2021 01:46:16 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:53:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:53:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Aug 2021 05:06:02 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 05:06:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 18 Aug 2021 05:06:05 GMT
ENV TELEGRAF_VERSION=1.17.3
# Wed, 18 Aug 2021 05:06:08 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 18 Aug 2021 05:06:08 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 18 Aug 2021 05:06:09 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 18 Aug 2021 05:06:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 05:06:09 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b721438f56fc7c4bf10a9f9ac58d22b52d97c50353a44f531fb5b7a70314e642`  
		Last Modified: Tue, 17 Aug 2021 01:53:52 GMT  
		Size: 49.2 MB (49222362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268ad76519936dc02d53171a3a4ca6eea0fc0b8a93e97cde6138071fe0422825`  
		Last Modified: Tue, 17 Aug 2021 08:02:23 GMT  
		Size: 7.7 MB (7695203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c93fd903c94bd33e20edef5822d935ca9efd856e0b3d41b0849c1df8ac81a09`  
		Last Modified: Tue, 17 Aug 2021 08:02:24 GMT  
		Size: 10.0 MB (9984343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565d34c87c364517d34ad3b0cc55cc5ba5228ed3d524e7349b620cb41ed599a6`  
		Last Modified: Wed, 18 Aug 2021 05:06:56 GMT  
		Size: 17.3 MB (17268562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba78e60bcb30e04825f9773196e1cb82065b234a76f0a78f95741f5ddb78315`  
		Last Modified: Wed, 18 Aug 2021 05:06:53 GMT  
		Size: 2.9 KB (2904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd8ad01af3b455ce3fd73777a3bbdf0a98228f222bf700a0d041fc2241d592c`  
		Last Modified: Wed, 18 Aug 2021 05:06:57 GMT  
		Size: 21.1 MB (21051715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee55e1faadae2e9dcc179189357ce7c7e9dd047664de23f3374338e94561b06`  
		Last Modified: Wed, 18 Aug 2021 05:06:53 GMT  
		Size: 185.0 B  
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
$ docker pull telegraf@sha256:5d3090b5e4d8744d3f5013ba20bb756a4ddd039b0f4d029984659d8eb7423936
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
$ docker pull telegraf@sha256:3787fc1730c5cf84b2c9098a086ecc2ffcd943e2b9821e67f74960b7a326426f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.2 MB (105225274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2030074ffd2bf35bcff436742fff780f1ad2be6ab1b46298638951704cd515dc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:16 GMT
ADD file:9e7d801ba29c50f7388cf80395faef75e0b4db056e16d1117293539bda895467 in / 
# Tue, 17 Aug 2021 01:46:16 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:53:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:53:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Aug 2021 05:06:02 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 05:06:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 18 Aug 2021 05:06:05 GMT
ENV TELEGRAF_VERSION=1.17.3
# Wed, 18 Aug 2021 05:06:08 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 18 Aug 2021 05:06:08 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 18 Aug 2021 05:06:09 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 18 Aug 2021 05:06:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 05:06:09 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b721438f56fc7c4bf10a9f9ac58d22b52d97c50353a44f531fb5b7a70314e642`  
		Last Modified: Tue, 17 Aug 2021 01:53:52 GMT  
		Size: 49.2 MB (49222362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268ad76519936dc02d53171a3a4ca6eea0fc0b8a93e97cde6138071fe0422825`  
		Last Modified: Tue, 17 Aug 2021 08:02:23 GMT  
		Size: 7.7 MB (7695203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c93fd903c94bd33e20edef5822d935ca9efd856e0b3d41b0849c1df8ac81a09`  
		Last Modified: Tue, 17 Aug 2021 08:02:24 GMT  
		Size: 10.0 MB (9984343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565d34c87c364517d34ad3b0cc55cc5ba5228ed3d524e7349b620cb41ed599a6`  
		Last Modified: Wed, 18 Aug 2021 05:06:56 GMT  
		Size: 17.3 MB (17268562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba78e60bcb30e04825f9773196e1cb82065b234a76f0a78f95741f5ddb78315`  
		Last Modified: Wed, 18 Aug 2021 05:06:53 GMT  
		Size: 2.9 KB (2904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bd8ad01af3b455ce3fd73777a3bbdf0a98228f222bf700a0d041fc2241d592c`  
		Last Modified: Wed, 18 Aug 2021 05:06:57 GMT  
		Size: 21.1 MB (21051715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ee55e1faadae2e9dcc179189357ce7c7e9dd047664de23f3374338e94561b06`  
		Last Modified: Wed, 18 Aug 2021 05:06:53 GMT  
		Size: 185.0 B  
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
$ docker pull telegraf@sha256:b010c37cabc7311526300e6f26640de9536286ddcd7d6a49f7d9fd022de6291a
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
$ docker pull telegraf@sha256:b8913a3f4e448654305d0f7fb922e65b742991d122dce9e3f4e3c2d9f9dcd3ca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.1 MB (111147279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09e4c9f8e449c5fdf71c4d218644b911a10f1d9b16673490174a58b8c518fa66`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:16 GMT
ADD file:9e7d801ba29c50f7388cf80395faef75e0b4db056e16d1117293539bda895467 in / 
# Tue, 17 Aug 2021 01:46:16 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:53:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:53:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Aug 2021 05:06:02 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 05:06:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 18 Aug 2021 05:06:14 GMT
ENV TELEGRAF_VERSION=1.18.3
# Wed, 18 Aug 2021 05:06:18 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 18 Aug 2021 05:06:18 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 18 Aug 2021 05:06:19 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 18 Aug 2021 05:06:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 05:06:19 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b721438f56fc7c4bf10a9f9ac58d22b52d97c50353a44f531fb5b7a70314e642`  
		Last Modified: Tue, 17 Aug 2021 01:53:52 GMT  
		Size: 49.2 MB (49222362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268ad76519936dc02d53171a3a4ca6eea0fc0b8a93e97cde6138071fe0422825`  
		Last Modified: Tue, 17 Aug 2021 08:02:23 GMT  
		Size: 7.7 MB (7695203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c93fd903c94bd33e20edef5822d935ca9efd856e0b3d41b0849c1df8ac81a09`  
		Last Modified: Tue, 17 Aug 2021 08:02:24 GMT  
		Size: 10.0 MB (9984343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565d34c87c364517d34ad3b0cc55cc5ba5228ed3d524e7349b620cb41ed599a6`  
		Last Modified: Wed, 18 Aug 2021 05:06:56 GMT  
		Size: 17.3 MB (17268562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba78e60bcb30e04825f9773196e1cb82065b234a76f0a78f95741f5ddb78315`  
		Last Modified: Wed, 18 Aug 2021 05:06:53 GMT  
		Size: 2.9 KB (2904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fefa5facfad934fedce27530f29cfacaa3c846cf7c95e2080c872230d7c32e76`  
		Last Modified: Wed, 18 Aug 2021 05:07:14 GMT  
		Size: 27.0 MB (26973720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db1aefd53110771f5aef1337e9633770740b217f120a7027777b0663798eec4`  
		Last Modified: Wed, 18 Aug 2021 05:07:09 GMT  
		Size: 185.0 B  
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
$ docker pull telegraf@sha256:b010c37cabc7311526300e6f26640de9536286ddcd7d6a49f7d9fd022de6291a
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
$ docker pull telegraf@sha256:b8913a3f4e448654305d0f7fb922e65b742991d122dce9e3f4e3c2d9f9dcd3ca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.1 MB (111147279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09e4c9f8e449c5fdf71c4d218644b911a10f1d9b16673490174a58b8c518fa66`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:16 GMT
ADD file:9e7d801ba29c50f7388cf80395faef75e0b4db056e16d1117293539bda895467 in / 
# Tue, 17 Aug 2021 01:46:16 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:53:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:53:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Aug 2021 05:06:02 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 05:06:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 18 Aug 2021 05:06:14 GMT
ENV TELEGRAF_VERSION=1.18.3
# Wed, 18 Aug 2021 05:06:18 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 18 Aug 2021 05:06:18 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 18 Aug 2021 05:06:19 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 18 Aug 2021 05:06:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 05:06:19 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b721438f56fc7c4bf10a9f9ac58d22b52d97c50353a44f531fb5b7a70314e642`  
		Last Modified: Tue, 17 Aug 2021 01:53:52 GMT  
		Size: 49.2 MB (49222362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268ad76519936dc02d53171a3a4ca6eea0fc0b8a93e97cde6138071fe0422825`  
		Last Modified: Tue, 17 Aug 2021 08:02:23 GMT  
		Size: 7.7 MB (7695203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c93fd903c94bd33e20edef5822d935ca9efd856e0b3d41b0849c1df8ac81a09`  
		Last Modified: Tue, 17 Aug 2021 08:02:24 GMT  
		Size: 10.0 MB (9984343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565d34c87c364517d34ad3b0cc55cc5ba5228ed3d524e7349b620cb41ed599a6`  
		Last Modified: Wed, 18 Aug 2021 05:06:56 GMT  
		Size: 17.3 MB (17268562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba78e60bcb30e04825f9773196e1cb82065b234a76f0a78f95741f5ddb78315`  
		Last Modified: Wed, 18 Aug 2021 05:06:53 GMT  
		Size: 2.9 KB (2904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fefa5facfad934fedce27530f29cfacaa3c846cf7c95e2080c872230d7c32e76`  
		Last Modified: Wed, 18 Aug 2021 05:07:14 GMT  
		Size: 27.0 MB (26973720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db1aefd53110771f5aef1337e9633770740b217f120a7027777b0663798eec4`  
		Last Modified: Wed, 18 Aug 2021 05:07:09 GMT  
		Size: 185.0 B  
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
$ docker pull telegraf@sha256:2984db593ab66a4df16cc4311f9917e4c5133d80352d9ae38fbce2ebe478cf43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.19` - linux; amd64

```console
$ docker pull telegraf@sha256:1793d98ab1ee6c804cacd66fd9b3d8111d371afa97b05b8261c2ce881a05da1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119755532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3292ebb7fef7621621405b8746432842dde3382623a9b4ab5726fbbcc56066a`
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
# Fri, 30 Jul 2021 00:21:14 GMT
ENV TELEGRAF_VERSION=1.19.2
# Fri, 30 Jul 2021 00:21:18 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 30 Jul 2021 00:21:19 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 30 Jul 2021 00:21:19 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 30 Jul 2021 00:21:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 30 Jul 2021 00:21:19 GMT
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
	-	`sha256:af47751f1357381e65b3e5bde13104c360fcbad161bb4fca08a282273f28c03f`  
		Last Modified: Fri, 30 Jul 2021 00:21:59 GMT  
		Size: 34.1 MB (34071497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6949a180ee75fec10cb8e698c34d2504842f9916742197032894c13ada67ea56`  
		Last Modified: Fri, 30 Jul 2021 00:21:53 GMT  
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
$ docker pull telegraf@sha256:164f8965f22c281c4e301661847efcd5d79453e00a16449314e623098721cb4e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.0 MB (115031849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3674daa4ad68474b5ec27f5688b784a882b860b4e19c8bc303ea3faef0c8119e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:16 GMT
ADD file:9e7d801ba29c50f7388cf80395faef75e0b4db056e16d1117293539bda895467 in / 
# Tue, 17 Aug 2021 01:46:16 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:53:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:53:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Aug 2021 05:06:02 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 05:06:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 18 Aug 2021 05:06:24 GMT
ENV TELEGRAF_VERSION=1.19.2
# Wed, 18 Aug 2021 05:06:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 18 Aug 2021 05:06:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 18 Aug 2021 05:06:29 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 18 Aug 2021 05:06:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 05:06:29 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b721438f56fc7c4bf10a9f9ac58d22b52d97c50353a44f531fb5b7a70314e642`  
		Last Modified: Tue, 17 Aug 2021 01:53:52 GMT  
		Size: 49.2 MB (49222362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268ad76519936dc02d53171a3a4ca6eea0fc0b8a93e97cde6138071fe0422825`  
		Last Modified: Tue, 17 Aug 2021 08:02:23 GMT  
		Size: 7.7 MB (7695203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c93fd903c94bd33e20edef5822d935ca9efd856e0b3d41b0849c1df8ac81a09`  
		Last Modified: Tue, 17 Aug 2021 08:02:24 GMT  
		Size: 10.0 MB (9984343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565d34c87c364517d34ad3b0cc55cc5ba5228ed3d524e7349b620cb41ed599a6`  
		Last Modified: Wed, 18 Aug 2021 05:06:56 GMT  
		Size: 17.3 MB (17268562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba78e60bcb30e04825f9773196e1cb82065b234a76f0a78f95741f5ddb78315`  
		Last Modified: Wed, 18 Aug 2021 05:06:53 GMT  
		Size: 2.9 KB (2904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c5efe21cd4049fd7b1fc94194543068ecfda406c6c2ab4d2bafd9665867630`  
		Last Modified: Wed, 18 Aug 2021 05:07:32 GMT  
		Size: 30.9 MB (30858291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0788055a9f36567d5d60243c75950f44211329862c0fde806fcd2bccd588690c`  
		Last Modified: Wed, 18 Aug 2021 05:07:26 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.19-alpine`

```console
$ docker pull telegraf@sha256:92bd53d143556916f65c3460bd045b11cc83b5812b8ffc1f9f0605a7168745b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.19-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:61c6a4bb2efccb2528b0446aa10d424b9c599585d0a7e0d7637c507856f50310
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (40020656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47d5db184d82326d77a46c955b240cb8eb2275df2f7a6b997df2f4b3e17976e7`
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
# Fri, 30 Jul 2021 00:21:22 GMT
ENV TELEGRAF_VERSION=1.19.2
# Fri, 30 Jul 2021 00:21:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 30 Jul 2021 00:21:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 30 Jul 2021 00:21:29 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Fri, 30 Jul 2021 00:21:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 30 Jul 2021 00:21:29 GMT
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
	-	`sha256:a602346b3bad87cf15e4fd1c2d7216530979a32c878b5ce666f68dd2950cf44b`  
		Last Modified: Fri, 30 Jul 2021 00:22:20 GMT  
		Size: 33.9 MB (33919079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666653330d219696ee19c7fbf99ce2b63ed96149d025971c599a7f8441e8a842`  
		Last Modified: Fri, 30 Jul 2021 00:22:12 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.19.2`

```console
$ docker pull telegraf@sha256:2984db593ab66a4df16cc4311f9917e4c5133d80352d9ae38fbce2ebe478cf43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.19.2` - linux; amd64

```console
$ docker pull telegraf@sha256:1793d98ab1ee6c804cacd66fd9b3d8111d371afa97b05b8261c2ce881a05da1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119755532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3292ebb7fef7621621405b8746432842dde3382623a9b4ab5726fbbcc56066a`
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
# Fri, 30 Jul 2021 00:21:14 GMT
ENV TELEGRAF_VERSION=1.19.2
# Fri, 30 Jul 2021 00:21:18 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 30 Jul 2021 00:21:19 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 30 Jul 2021 00:21:19 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 30 Jul 2021 00:21:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 30 Jul 2021 00:21:19 GMT
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
	-	`sha256:af47751f1357381e65b3e5bde13104c360fcbad161bb4fca08a282273f28c03f`  
		Last Modified: Fri, 30 Jul 2021 00:21:59 GMT  
		Size: 34.1 MB (34071497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6949a180ee75fec10cb8e698c34d2504842f9916742197032894c13ada67ea56`  
		Last Modified: Fri, 30 Jul 2021 00:21:53 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

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
$ docker pull telegraf@sha256:164f8965f22c281c4e301661847efcd5d79453e00a16449314e623098721cb4e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.0 MB (115031849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3674daa4ad68474b5ec27f5688b784a882b860b4e19c8bc303ea3faef0c8119e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:16 GMT
ADD file:9e7d801ba29c50f7388cf80395faef75e0b4db056e16d1117293539bda895467 in / 
# Tue, 17 Aug 2021 01:46:16 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:53:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:53:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Aug 2021 05:06:02 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 05:06:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 18 Aug 2021 05:06:24 GMT
ENV TELEGRAF_VERSION=1.19.2
# Wed, 18 Aug 2021 05:06:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 18 Aug 2021 05:06:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 18 Aug 2021 05:06:29 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 18 Aug 2021 05:06:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 05:06:29 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b721438f56fc7c4bf10a9f9ac58d22b52d97c50353a44f531fb5b7a70314e642`  
		Last Modified: Tue, 17 Aug 2021 01:53:52 GMT  
		Size: 49.2 MB (49222362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268ad76519936dc02d53171a3a4ca6eea0fc0b8a93e97cde6138071fe0422825`  
		Last Modified: Tue, 17 Aug 2021 08:02:23 GMT  
		Size: 7.7 MB (7695203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c93fd903c94bd33e20edef5822d935ca9efd856e0b3d41b0849c1df8ac81a09`  
		Last Modified: Tue, 17 Aug 2021 08:02:24 GMT  
		Size: 10.0 MB (9984343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565d34c87c364517d34ad3b0cc55cc5ba5228ed3d524e7349b620cb41ed599a6`  
		Last Modified: Wed, 18 Aug 2021 05:06:56 GMT  
		Size: 17.3 MB (17268562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba78e60bcb30e04825f9773196e1cb82065b234a76f0a78f95741f5ddb78315`  
		Last Modified: Wed, 18 Aug 2021 05:06:53 GMT  
		Size: 2.9 KB (2904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c5efe21cd4049fd7b1fc94194543068ecfda406c6c2ab4d2bafd9665867630`  
		Last Modified: Wed, 18 Aug 2021 05:07:32 GMT  
		Size: 30.9 MB (30858291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0788055a9f36567d5d60243c75950f44211329862c0fde806fcd2bccd588690c`  
		Last Modified: Wed, 18 Aug 2021 05:07:26 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.19.2-alpine`

```console
$ docker pull telegraf@sha256:92bd53d143556916f65c3460bd045b11cc83b5812b8ffc1f9f0605a7168745b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.19.2-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:61c6a4bb2efccb2528b0446aa10d424b9c599585d0a7e0d7637c507856f50310
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (40020656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47d5db184d82326d77a46c955b240cb8eb2275df2f7a6b997df2f4b3e17976e7`
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
# Fri, 30 Jul 2021 00:21:22 GMT
ENV TELEGRAF_VERSION=1.19.2
# Fri, 30 Jul 2021 00:21:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 30 Jul 2021 00:21:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 30 Jul 2021 00:21:29 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Fri, 30 Jul 2021 00:21:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 30 Jul 2021 00:21:29 GMT
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
	-	`sha256:a602346b3bad87cf15e4fd1c2d7216530979a32c878b5ce666f68dd2950cf44b`  
		Last Modified: Fri, 30 Jul 2021 00:22:20 GMT  
		Size: 33.9 MB (33919079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666653330d219696ee19c7fbf99ce2b63ed96149d025971c599a7f8441e8a842`  
		Last Modified: Fri, 30 Jul 2021 00:22:12 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:92bd53d143556916f65c3460bd045b11cc83b5812b8ffc1f9f0605a7168745b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:61c6a4bb2efccb2528b0446aa10d424b9c599585d0a7e0d7637c507856f50310
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (40020656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47d5db184d82326d77a46c955b240cb8eb2275df2f7a6b997df2f4b3e17976e7`
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
# Fri, 30 Jul 2021 00:21:22 GMT
ENV TELEGRAF_VERSION=1.19.2
# Fri, 30 Jul 2021 00:21:28 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 30 Jul 2021 00:21:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 30 Jul 2021 00:21:29 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Fri, 30 Jul 2021 00:21:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 30 Jul 2021 00:21:29 GMT
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
	-	`sha256:a602346b3bad87cf15e4fd1c2d7216530979a32c878b5ce666f68dd2950cf44b`  
		Last Modified: Fri, 30 Jul 2021 00:22:20 GMT  
		Size: 33.9 MB (33919079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666653330d219696ee19c7fbf99ce2b63ed96149d025971c599a7f8441e8a842`  
		Last Modified: Fri, 30 Jul 2021 00:22:12 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:2984db593ab66a4df16cc4311f9917e4c5133d80352d9ae38fbce2ebe478cf43
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:1793d98ab1ee6c804cacd66fd9b3d8111d371afa97b05b8261c2ce881a05da1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.8 MB (119755532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3292ebb7fef7621621405b8746432842dde3382623a9b4ab5726fbbcc56066a`
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
# Fri, 30 Jul 2021 00:21:14 GMT
ENV TELEGRAF_VERSION=1.19.2
# Fri, 30 Jul 2021 00:21:18 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 30 Jul 2021 00:21:19 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 30 Jul 2021 00:21:19 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Fri, 30 Jul 2021 00:21:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 30 Jul 2021 00:21:19 GMT
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
	-	`sha256:af47751f1357381e65b3e5bde13104c360fcbad161bb4fca08a282273f28c03f`  
		Last Modified: Fri, 30 Jul 2021 00:21:59 GMT  
		Size: 34.1 MB (34071497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6949a180ee75fec10cb8e698c34d2504842f9916742197032894c13ada67ea56`  
		Last Modified: Fri, 30 Jul 2021 00:21:53 GMT  
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
$ docker pull telegraf@sha256:164f8965f22c281c4e301661847efcd5d79453e00a16449314e623098721cb4e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.0 MB (115031849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3674daa4ad68474b5ec27f5688b784a882b860b4e19c8bc303ea3faef0c8119e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 17 Aug 2021 01:46:16 GMT
ADD file:9e7d801ba29c50f7388cf80395faef75e0b4db056e16d1117293539bda895467 in / 
# Tue, 17 Aug 2021 01:46:16 GMT
CMD ["bash"]
# Tue, 17 Aug 2021 07:53:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 17 Aug 2021 07:53:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Aug 2021 05:06:02 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 18 Aug 2021 05:06:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 18 Aug 2021 05:06:24 GMT
ENV TELEGRAF_VERSION=1.19.2
# Wed, 18 Aug 2021 05:06:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 18 Aug 2021 05:06:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 18 Aug 2021 05:06:29 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 18 Aug 2021 05:06:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Aug 2021 05:06:29 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b721438f56fc7c4bf10a9f9ac58d22b52d97c50353a44f531fb5b7a70314e642`  
		Last Modified: Tue, 17 Aug 2021 01:53:52 GMT  
		Size: 49.2 MB (49222362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268ad76519936dc02d53171a3a4ca6eea0fc0b8a93e97cde6138071fe0422825`  
		Last Modified: Tue, 17 Aug 2021 08:02:23 GMT  
		Size: 7.7 MB (7695203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c93fd903c94bd33e20edef5822d935ca9efd856e0b3d41b0849c1df8ac81a09`  
		Last Modified: Tue, 17 Aug 2021 08:02:24 GMT  
		Size: 10.0 MB (9984343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565d34c87c364517d34ad3b0cc55cc5ba5228ed3d524e7349b620cb41ed599a6`  
		Last Modified: Wed, 18 Aug 2021 05:06:56 GMT  
		Size: 17.3 MB (17268562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba78e60bcb30e04825f9773196e1cb82065b234a76f0a78f95741f5ddb78315`  
		Last Modified: Wed, 18 Aug 2021 05:06:53 GMT  
		Size: 2.9 KB (2904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1c5efe21cd4049fd7b1fc94194543068ecfda406c6c2ab4d2bafd9665867630`  
		Last Modified: Wed, 18 Aug 2021 05:07:32 GMT  
		Size: 30.9 MB (30858291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0788055a9f36567d5d60243c75950f44211329862c0fde806fcd2bccd588690c`  
		Last Modified: Wed, 18 Aug 2021 05:07:26 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
