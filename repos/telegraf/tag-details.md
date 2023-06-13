<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `telegraf`

-	[`telegraf:1.25`](#telegraf125)
-	[`telegraf:1.25-alpine`](#telegraf125-alpine)
-	[`telegraf:1.25.3`](#telegraf1253)
-	[`telegraf:1.25.3-alpine`](#telegraf1253-alpine)
-	[`telegraf:1.26`](#telegraf126)
-	[`telegraf:1.26-alpine`](#telegraf126-alpine)
-	[`telegraf:1.26.3`](#telegraf1263)
-	[`telegraf:1.26.3-alpine`](#telegraf1263-alpine)
-	[`telegraf:1.27`](#telegraf127)
-	[`telegraf:1.27-alpine`](#telegraf127-alpine)
-	[`telegraf:1.27.0`](#telegraf1270)
-	[`telegraf:1.27.0-alpine`](#telegraf1270-alpine)
-	[`telegraf:alpine`](#telegrafalpine)
-	[`telegraf:latest`](#telegraflatest)

## `telegraf:1.25`

```console
$ docker pull telegraf@sha256:1bc461215b07a7dda87b7015b593a7e69b0f0dedb5ec13f981d011694ce60102
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.25` - linux; amd64

```console
$ docker pull telegraf@sha256:91490638387645e4c9f9f16ef7b54fd170cf4bd46bf0916129d352c1144c1b22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.1 MB (136148209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a675959b31710de1af35a7fd46823eb89818861d1e5df724d1637a70c652caf2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 May 2023 01:20:00 GMT
ADD file:150a6453ab2258061c1a1549ab119df752bdc2c2c84028fa0e83a0663cd8cedf in / 
# Tue, 23 May 2023 01:20:01 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:48:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 20:36:19 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 20:36:21 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 23 May 2023 20:36:30 GMT
ENV TELEGRAF_VERSION=1.25.3
# Tue, 23 May 2023 20:36:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 23 May 2023 20:36:34 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 23 May 2023 20:36:34 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 23 May 2023 20:36:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 May 2023 20:36:34 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:bd73737482dd5575526c7207872963479808d979ab2741c321706b8553918474`  
		Last Modified: Tue, 23 May 2023 01:23:46 GMT  
		Size: 55.0 MB (55049027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6710592d62aa1338ac1c1c363dedc255659f666cc41441c7e0f735c484db10ff`  
		Last Modified: Tue, 23 May 2023 01:56:06 GMT  
		Size: 15.8 MB (15760489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342d6d3ae9d9daf15efede898e8707fb9967951505106804ac53dd29f5e0f0ae`  
		Last Modified: Tue, 23 May 2023 20:36:59 GMT  
		Size: 18.8 MB (18759968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b674984b48670e73e773310e315a978db8ed074adccaff1f0152f6fa88914a43`  
		Last Modified: Tue, 23 May 2023 20:36:57 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accac8026ce920efa42295e70f6ed7211e9ad03e53c8fc7671f6036d3ba80e08`  
		Last Modified: Tue, 23 May 2023 20:37:19 GMT  
		Size: 46.6 MB (46576587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f6ba36261cf993408720d8e5464597cc8774e544e685c24d94832fb219db4b`  
		Last Modified: Tue, 23 May 2023 20:37:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:e279060b7c8fcd16d15873220038a8821d76c430476b37547aac9f29e131d66f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125927008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7a35d70722d1fcfe2669a9c6c281d61018a9f1a6cc32b99d9ee0a55497839d5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 May 2023 00:57:45 GMT
ADD file:d8748d34e524d93a6df76d2a8ea8ca32ca04897521719f9f1f2a88ec692dd69e in / 
# Tue, 23 May 2023 00:57:45 GMT
CMD ["bash"]
# Tue, 23 May 2023 09:54:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 23:16:17 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 23:16:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 23 May 2023 23:16:28 GMT
ENV TELEGRAF_VERSION=1.25.3
# Tue, 23 May 2023 23:16:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 23 May 2023 23:16:35 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 23 May 2023 23:16:35 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 23 May 2023 23:16:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 May 2023 23:16:35 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:29949e2d07dd1e283862cb4c3d4ec3043f1d54a1ac59f7b7a998ed9038a0243c`  
		Last Modified: Tue, 23 May 2023 01:01:23 GMT  
		Size: 50.2 MB (50210000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aaf40f65a7bdc041e615a5825b6ae62227f6a7ceec53af9e210fb62293e0bd2`  
		Last Modified: Tue, 23 May 2023 10:04:45 GMT  
		Size: 14.9 MB (14868582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fa44955cadb3e3d3d5fe86d27c4488b7e7aac3646248014cc6911ff7195039`  
		Last Modified: Tue, 23 May 2023 23:16:55 GMT  
		Size: 17.5 MB (17462338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e198f55fd4a95bb93ec5e99c99bf326613e1a6bad919dda290b804d7b627934`  
		Last Modified: Tue, 23 May 2023 23:16:52 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3bd5df417d74eb9fb77d3add1d41dce76e0a927ffc17b213fb66e4b5ad5f62`  
		Last Modified: Tue, 23 May 2023 23:17:15 GMT  
		Size: 43.4 MB (43383939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34451c0b8d62f4e8e2c0110b667c03b2e3daeb3c89299a0f67b754b552a6b7a6`  
		Last Modified: Tue, 23 May 2023 23:17:08 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:54ec56e7dbff1ec3d9bc663a62e4177a1c18e4708960905ee1dc62979009fb77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130366398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:075ee8da9c64e3190004132888b2a46af12e61d87ece9016dfce207dc27701b7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:01:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:32:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:32:06 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 18:32:06 GMT
ENV TELEGRAF_VERSION=1.25.3
# Tue, 13 Jun 2023 18:32:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Jun 2023 18:32:15 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Jun 2023 18:32:15 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Jun 2023 18:32:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 18:32:15 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751c9c60873892c6128382a04355bf76576dd23d87e5fdad03161dba5a2db45e`  
		Last Modified: Tue, 13 Jun 2023 03:08:33 GMT  
		Size: 15.7 MB (15746563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f7beb564cd4e17ac6f0066d8923c3e1a33cf5131542c873cd289e83bc2f98d`  
		Last Modified: Tue, 13 Jun 2023 18:32:50 GMT  
		Size: 18.6 MB (18598375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73606481ffac7e00171316db43e6998cf7b12ad1484bf62c4f7da607957b601`  
		Last Modified: Tue, 13 Jun 2023 18:32:47 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac998d375180a9e7c51227843060265390355e20d83805f2a432f9814e36a64`  
		Last Modified: Tue, 13 Jun 2023 18:32:52 GMT  
		Size: 42.3 MB (42315175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c07b237814b62dd8776167685850a8cf11e305dbb7e06fc02ac4ed0c562451d`  
		Last Modified: Tue, 13 Jun 2023 18:32:47 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25-alpine`

```console
$ docker pull telegraf@sha256:ac9a4e47c138874f0c2952e42e36a30ce2f2fcf0fe69a01f21bf7ac69963eb1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.25-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:47a1cf60e5d34ef5df582e82d56a0074acdf15434fec9731aad5edea15206f5b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52439134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42cd0e4d80e349dd061253e36708fc572e20e2b46b20299b68ee6fb2b5f22099`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Mar 2023 02:39:58 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Thu, 30 Mar 2023 02:40:09 GMT
ENV TELEGRAF_VERSION=1.25.3
# Thu, 30 Mar 2023 02:40:17 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Thu, 30 Mar 2023 02:40:17 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 30 Mar 2023 02:40:17 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Thu, 30 Mar 2023 02:40:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 02:40:17 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc4e566a0dbfe02f4f43cee08d69aba4ae1fac7498203229b86614b5d893657`  
		Last Modified: Thu, 30 Mar 2023 02:40:39 GMT  
		Size: 2.7 MB (2671310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774523858861fcfca4026bb49b6c20abe09bea753f173786f31e5241e313b890`  
		Last Modified: Thu, 30 Mar 2023 02:41:00 GMT  
		Size: 46.4 MB (46392656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fe8ce1c7509c7c03c0cdd600fe009678b277043c50973b5915a54e3a78f04e`  
		Last Modified: Thu, 30 Mar 2023 02:40:53 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25.3`

```console
$ docker pull telegraf@sha256:1bc461215b07a7dda87b7015b593a7e69b0f0dedb5ec13f981d011694ce60102
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.25.3` - linux; amd64

```console
$ docker pull telegraf@sha256:91490638387645e4c9f9f16ef7b54fd170cf4bd46bf0916129d352c1144c1b22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.1 MB (136148209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a675959b31710de1af35a7fd46823eb89818861d1e5df724d1637a70c652caf2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 May 2023 01:20:00 GMT
ADD file:150a6453ab2258061c1a1549ab119df752bdc2c2c84028fa0e83a0663cd8cedf in / 
# Tue, 23 May 2023 01:20:01 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:48:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 20:36:19 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 20:36:21 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 23 May 2023 20:36:30 GMT
ENV TELEGRAF_VERSION=1.25.3
# Tue, 23 May 2023 20:36:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 23 May 2023 20:36:34 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 23 May 2023 20:36:34 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 23 May 2023 20:36:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 May 2023 20:36:34 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:bd73737482dd5575526c7207872963479808d979ab2741c321706b8553918474`  
		Last Modified: Tue, 23 May 2023 01:23:46 GMT  
		Size: 55.0 MB (55049027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6710592d62aa1338ac1c1c363dedc255659f666cc41441c7e0f735c484db10ff`  
		Last Modified: Tue, 23 May 2023 01:56:06 GMT  
		Size: 15.8 MB (15760489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342d6d3ae9d9daf15efede898e8707fb9967951505106804ac53dd29f5e0f0ae`  
		Last Modified: Tue, 23 May 2023 20:36:59 GMT  
		Size: 18.8 MB (18759968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b674984b48670e73e773310e315a978db8ed074adccaff1f0152f6fa88914a43`  
		Last Modified: Tue, 23 May 2023 20:36:57 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:accac8026ce920efa42295e70f6ed7211e9ad03e53c8fc7671f6036d3ba80e08`  
		Last Modified: Tue, 23 May 2023 20:37:19 GMT  
		Size: 46.6 MB (46576587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f6ba36261cf993408720d8e5464597cc8774e544e685c24d94832fb219db4b`  
		Last Modified: Tue, 23 May 2023 20:37:12 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25.3` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:e279060b7c8fcd16d15873220038a8821d76c430476b37547aac9f29e131d66f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125927008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7a35d70722d1fcfe2669a9c6c281d61018a9f1a6cc32b99d9ee0a55497839d5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 May 2023 00:57:45 GMT
ADD file:d8748d34e524d93a6df76d2a8ea8ca32ca04897521719f9f1f2a88ec692dd69e in / 
# Tue, 23 May 2023 00:57:45 GMT
CMD ["bash"]
# Tue, 23 May 2023 09:54:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 23:16:17 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 23:16:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 23 May 2023 23:16:28 GMT
ENV TELEGRAF_VERSION=1.25.3
# Tue, 23 May 2023 23:16:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 23 May 2023 23:16:35 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 23 May 2023 23:16:35 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 23 May 2023 23:16:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 May 2023 23:16:35 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:29949e2d07dd1e283862cb4c3d4ec3043f1d54a1ac59f7b7a998ed9038a0243c`  
		Last Modified: Tue, 23 May 2023 01:01:23 GMT  
		Size: 50.2 MB (50210000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aaf40f65a7bdc041e615a5825b6ae62227f6a7ceec53af9e210fb62293e0bd2`  
		Last Modified: Tue, 23 May 2023 10:04:45 GMT  
		Size: 14.9 MB (14868582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fa44955cadb3e3d3d5fe86d27c4488b7e7aac3646248014cc6911ff7195039`  
		Last Modified: Tue, 23 May 2023 23:16:55 GMT  
		Size: 17.5 MB (17462338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e198f55fd4a95bb93ec5e99c99bf326613e1a6bad919dda290b804d7b627934`  
		Last Modified: Tue, 23 May 2023 23:16:52 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3bd5df417d74eb9fb77d3add1d41dce76e0a927ffc17b213fb66e4b5ad5f62`  
		Last Modified: Tue, 23 May 2023 23:17:15 GMT  
		Size: 43.4 MB (43383939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34451c0b8d62f4e8e2c0110b667c03b2e3daeb3c89299a0f67b754b552a6b7a6`  
		Last Modified: Tue, 23 May 2023 23:17:08 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25.3` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:54ec56e7dbff1ec3d9bc663a62e4177a1c18e4708960905ee1dc62979009fb77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130366398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:075ee8da9c64e3190004132888b2a46af12e61d87ece9016dfce207dc27701b7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:01:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:32:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:32:06 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 18:32:06 GMT
ENV TELEGRAF_VERSION=1.25.3
# Tue, 13 Jun 2023 18:32:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Jun 2023 18:32:15 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Jun 2023 18:32:15 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Jun 2023 18:32:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 18:32:15 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751c9c60873892c6128382a04355bf76576dd23d87e5fdad03161dba5a2db45e`  
		Last Modified: Tue, 13 Jun 2023 03:08:33 GMT  
		Size: 15.7 MB (15746563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f7beb564cd4e17ac6f0066d8923c3e1a33cf5131542c873cd289e83bc2f98d`  
		Last Modified: Tue, 13 Jun 2023 18:32:50 GMT  
		Size: 18.6 MB (18598375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73606481ffac7e00171316db43e6998cf7b12ad1484bf62c4f7da607957b601`  
		Last Modified: Tue, 13 Jun 2023 18:32:47 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac998d375180a9e7c51227843060265390355e20d83805f2a432f9814e36a64`  
		Last Modified: Tue, 13 Jun 2023 18:32:52 GMT  
		Size: 42.3 MB (42315175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c07b237814b62dd8776167685850a8cf11e305dbb7e06fc02ac4ed0c562451d`  
		Last Modified: Tue, 13 Jun 2023 18:32:47 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25.3-alpine`

```console
$ docker pull telegraf@sha256:ac9a4e47c138874f0c2952e42e36a30ce2f2fcf0fe69a01f21bf7ac69963eb1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.25.3-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:47a1cf60e5d34ef5df582e82d56a0074acdf15434fec9731aad5edea15206f5b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52439134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42cd0e4d80e349dd061253e36708fc572e20e2b46b20299b68ee6fb2b5f22099`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Mar 2023 02:39:58 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Thu, 30 Mar 2023 02:40:09 GMT
ENV TELEGRAF_VERSION=1.25.3
# Thu, 30 Mar 2023 02:40:17 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Thu, 30 Mar 2023 02:40:17 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 30 Mar 2023 02:40:17 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Thu, 30 Mar 2023 02:40:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 02:40:17 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc4e566a0dbfe02f4f43cee08d69aba4ae1fac7498203229b86614b5d893657`  
		Last Modified: Thu, 30 Mar 2023 02:40:39 GMT  
		Size: 2.7 MB (2671310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:774523858861fcfca4026bb49b6c20abe09bea753f173786f31e5241e313b890`  
		Last Modified: Thu, 30 Mar 2023 02:41:00 GMT  
		Size: 46.4 MB (46392656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86fe8ce1c7509c7c03c0cdd600fe009678b277043c50973b5915a54e3a78f04e`  
		Last Modified: Thu, 30 Mar 2023 02:40:53 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26`

```console
$ docker pull telegraf@sha256:89bce574b401ce2d40e3bbe35fefc92c5fcbb8ea30462848680d926174c8eb70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.26` - linux; amd64

```console
$ docker pull telegraf@sha256:b68b2b342f4ab7fb658aa7e8cdb2c02148f4342091aed9790103e9226d8dcfa9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140124135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7b0598b10601106a0b43398cbe2fce04915b7ca0a56f86c5b3dcfcec8b93bd2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 May 2023 01:20:00 GMT
ADD file:150a6453ab2258061c1a1549ab119df752bdc2c2c84028fa0e83a0663cd8cedf in / 
# Tue, 23 May 2023 01:20:01 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:48:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 20:36:19 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 20:36:21 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 23 May 2023 20:36:39 GMT
ENV TELEGRAF_VERSION=1.26.3
# Tue, 23 May 2023 20:36:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 23 May 2023 20:36:43 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 23 May 2023 20:36:43 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 23 May 2023 20:36:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 May 2023 20:36:43 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:bd73737482dd5575526c7207872963479808d979ab2741c321706b8553918474`  
		Last Modified: Tue, 23 May 2023 01:23:46 GMT  
		Size: 55.0 MB (55049027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6710592d62aa1338ac1c1c363dedc255659f666cc41441c7e0f735c484db10ff`  
		Last Modified: Tue, 23 May 2023 01:56:06 GMT  
		Size: 15.8 MB (15760489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342d6d3ae9d9daf15efede898e8707fb9967951505106804ac53dd29f5e0f0ae`  
		Last Modified: Tue, 23 May 2023 20:36:59 GMT  
		Size: 18.8 MB (18759968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b674984b48670e73e773310e315a978db8ed074adccaff1f0152f6fa88914a43`  
		Last Modified: Tue, 23 May 2023 20:36:57 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68214bc12b63b670b91099b1d1842c85fd1b17735e412b7aea8f0748e7616047`  
		Last Modified: Tue, 23 May 2023 20:37:36 GMT  
		Size: 50.6 MB (50552512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275cc6e47c44a2ee8324d298fe11eab760699d3cd2aa42ef869dea0af87d7192`  
		Last Modified: Tue, 23 May 2023 20:37:29 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:90a928b95210ced28f7a90d30324e38e556151ffb4291d657591eaa3dbfac9d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129825789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c8072fdb2ecae58d07f598fde639c48404656fa420e8a1c3c5c8cde982547ea`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 May 2023 00:57:45 GMT
ADD file:d8748d34e524d93a6df76d2a8ea8ca32ca04897521719f9f1f2a88ec692dd69e in / 
# Tue, 23 May 2023 00:57:45 GMT
CMD ["bash"]
# Tue, 23 May 2023 09:54:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 23:16:17 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 23:16:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 23 May 2023 23:16:37 GMT
ENV TELEGRAF_VERSION=1.26.3
# Tue, 23 May 2023 23:16:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 23 May 2023 23:16:43 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 23 May 2023 23:16:43 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 23 May 2023 23:16:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 May 2023 23:16:44 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:29949e2d07dd1e283862cb4c3d4ec3043f1d54a1ac59f7b7a998ed9038a0243c`  
		Last Modified: Tue, 23 May 2023 01:01:23 GMT  
		Size: 50.2 MB (50210000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aaf40f65a7bdc041e615a5825b6ae62227f6a7ceec53af9e210fb62293e0bd2`  
		Last Modified: Tue, 23 May 2023 10:04:45 GMT  
		Size: 14.9 MB (14868582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fa44955cadb3e3d3d5fe86d27c4488b7e7aac3646248014cc6911ff7195039`  
		Last Modified: Tue, 23 May 2023 23:16:55 GMT  
		Size: 17.5 MB (17462338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e198f55fd4a95bb93ec5e99c99bf326613e1a6bad919dda290b804d7b627934`  
		Last Modified: Tue, 23 May 2023 23:16:52 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e3fa3ecf227f1ebec3c55bd0f33660f55a4c72c7c98126866fdb24c8eeb994`  
		Last Modified: Tue, 23 May 2023 23:17:32 GMT  
		Size: 47.3 MB (47282718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4a035c4ce960fbf0c1cc8f49f3ae3a551717a393f49d9816680b83232429f2`  
		Last Modified: Tue, 23 May 2023 23:17:25 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:469c8395bc63238cbf8edbd03ee7fcfa1e612886983ae96ed3d01f5e2a161f63
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (134023049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3397e0751df6f6f99a3d83b78814985cdc24393e1908c11c7637c0600a5bec6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:01:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:32:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:32:06 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 18:32:17 GMT
ENV TELEGRAF_VERSION=1.26.3
# Tue, 13 Jun 2023 18:32:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Jun 2023 18:32:23 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Jun 2023 18:32:23 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Jun 2023 18:32:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 18:32:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751c9c60873892c6128382a04355bf76576dd23d87e5fdad03161dba5a2db45e`  
		Last Modified: Tue, 13 Jun 2023 03:08:33 GMT  
		Size: 15.7 MB (15746563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f7beb564cd4e17ac6f0066d8923c3e1a33cf5131542c873cd289e83bc2f98d`  
		Last Modified: Tue, 13 Jun 2023 18:32:50 GMT  
		Size: 18.6 MB (18598375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73606481ffac7e00171316db43e6998cf7b12ad1484bf62c4f7da607957b601`  
		Last Modified: Tue, 13 Jun 2023 18:32:47 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76673891e1d56c6ac4aeff9b37b2aba2292b7b4d707c24da4b6a620be7bf451c`  
		Last Modified: Tue, 13 Jun 2023 18:33:06 GMT  
		Size: 46.0 MB (45971825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780d64765ed31438940ad94e7d16ce89b012387a5f84b3b3650a8d7802125bd9`  
		Last Modified: Tue, 13 Jun 2023 18:33:01 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26-alpine`

```console
$ docker pull telegraf@sha256:bcc8de7293da7691bb01ae7d92d5028697c75326505ab952c77e3f30beb26e8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.26-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:4355ab72932e3c3458f983d3f4ec18b038a0e6555bbac3b78a3bda15fe0b097b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.4 MB (56438425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e1ba951eb6880d6b98c3f0aace8c3d03eeb423de7ed6be2e5de4a913fe5e97a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Mar 2023 02:39:58 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 22 May 2023 21:20:15 GMT
ENV TELEGRAF_VERSION=1.26.3
# Mon, 22 May 2023 21:20:21 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 22 May 2023 21:20:21 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 22 May 2023 21:20:22 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 22 May 2023 21:20:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 22 May 2023 21:20:22 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc4e566a0dbfe02f4f43cee08d69aba4ae1fac7498203229b86614b5d893657`  
		Last Modified: Thu, 30 Mar 2023 02:40:39 GMT  
		Size: 2.7 MB (2671310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840e49ac9f99eaec4020a3323146a8b2397c8db1cc172fa8a23508fa57667ba0`  
		Last Modified: Mon, 22 May 2023 21:21:03 GMT  
		Size: 50.4 MB (50391946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49481bb95fc2dde1fd38d56151df02d8be684e818fd3a2e72f65d5f274074515`  
		Last Modified: Mon, 22 May 2023 21:20:55 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:dc6bfbc3c98a8b50f8da8f65fc86bb36a3dab1f5a1c35c0141a70476fab5351a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51778071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80638ca136f6fff412e37d8a330474c503d0bfc1b1673bc77dbff94df832ca0c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:17:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Mar 2023 05:53:19 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 22 May 2023 20:51:12 GMT
ENV TELEGRAF_VERSION=1.26.3
# Mon, 22 May 2023 20:51:23 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 22 May 2023 20:51:24 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 22 May 2023 20:51:24 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 22 May 2023 20:51:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 22 May 2023 20:51:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed363db396bd455184362560a01cd691a111fe2dea827312e4f70ec9d621fee`  
		Last Modified: Thu, 30 Mar 2023 04:18:04 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667a1eb2ec7610bdd0add751f09715319b000a6f9d65d272224680b46dd4871b`  
		Last Modified: Thu, 30 Mar 2023 05:53:39 GMT  
		Size: 2.7 MB (2703331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ef0ba6ccd8cc39ee7047af6650f38b324fc134cd9b5c857d116a923c039f2d`  
		Last Modified: Mon, 22 May 2023 20:51:56 GMT  
		Size: 45.8 MB (45812280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb87779c95194a7e41abdfa9ffbc2da15f428fd56b1f87f491da22256a4c57a0`  
		Last Modified: Mon, 22 May 2023 20:51:51 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26.3`

```console
$ docker pull telegraf@sha256:89bce574b401ce2d40e3bbe35fefc92c5fcbb8ea30462848680d926174c8eb70
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.26.3` - linux; amd64

```console
$ docker pull telegraf@sha256:b68b2b342f4ab7fb658aa7e8cdb2c02148f4342091aed9790103e9226d8dcfa9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140124135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7b0598b10601106a0b43398cbe2fce04915b7ca0a56f86c5b3dcfcec8b93bd2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 May 2023 01:20:00 GMT
ADD file:150a6453ab2258061c1a1549ab119df752bdc2c2c84028fa0e83a0663cd8cedf in / 
# Tue, 23 May 2023 01:20:01 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:48:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 20:36:19 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 20:36:21 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 23 May 2023 20:36:39 GMT
ENV TELEGRAF_VERSION=1.26.3
# Tue, 23 May 2023 20:36:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 23 May 2023 20:36:43 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 23 May 2023 20:36:43 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 23 May 2023 20:36:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 May 2023 20:36:43 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:bd73737482dd5575526c7207872963479808d979ab2741c321706b8553918474`  
		Last Modified: Tue, 23 May 2023 01:23:46 GMT  
		Size: 55.0 MB (55049027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6710592d62aa1338ac1c1c363dedc255659f666cc41441c7e0f735c484db10ff`  
		Last Modified: Tue, 23 May 2023 01:56:06 GMT  
		Size: 15.8 MB (15760489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342d6d3ae9d9daf15efede898e8707fb9967951505106804ac53dd29f5e0f0ae`  
		Last Modified: Tue, 23 May 2023 20:36:59 GMT  
		Size: 18.8 MB (18759968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b674984b48670e73e773310e315a978db8ed074adccaff1f0152f6fa88914a43`  
		Last Modified: Tue, 23 May 2023 20:36:57 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68214bc12b63b670b91099b1d1842c85fd1b17735e412b7aea8f0748e7616047`  
		Last Modified: Tue, 23 May 2023 20:37:36 GMT  
		Size: 50.6 MB (50552512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:275cc6e47c44a2ee8324d298fe11eab760699d3cd2aa42ef869dea0af87d7192`  
		Last Modified: Tue, 23 May 2023 20:37:29 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26.3` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:90a928b95210ced28f7a90d30324e38e556151ffb4291d657591eaa3dbfac9d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129825789 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c8072fdb2ecae58d07f598fde639c48404656fa420e8a1c3c5c8cde982547ea`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 May 2023 00:57:45 GMT
ADD file:d8748d34e524d93a6df76d2a8ea8ca32ca04897521719f9f1f2a88ec692dd69e in / 
# Tue, 23 May 2023 00:57:45 GMT
CMD ["bash"]
# Tue, 23 May 2023 09:54:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 23:16:17 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 23:16:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 23 May 2023 23:16:37 GMT
ENV TELEGRAF_VERSION=1.26.3
# Tue, 23 May 2023 23:16:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 23 May 2023 23:16:43 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 23 May 2023 23:16:43 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 23 May 2023 23:16:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 May 2023 23:16:44 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:29949e2d07dd1e283862cb4c3d4ec3043f1d54a1ac59f7b7a998ed9038a0243c`  
		Last Modified: Tue, 23 May 2023 01:01:23 GMT  
		Size: 50.2 MB (50210000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aaf40f65a7bdc041e615a5825b6ae62227f6a7ceec53af9e210fb62293e0bd2`  
		Last Modified: Tue, 23 May 2023 10:04:45 GMT  
		Size: 14.9 MB (14868582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fa44955cadb3e3d3d5fe86d27c4488b7e7aac3646248014cc6911ff7195039`  
		Last Modified: Tue, 23 May 2023 23:16:55 GMT  
		Size: 17.5 MB (17462338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e198f55fd4a95bb93ec5e99c99bf326613e1a6bad919dda290b804d7b627934`  
		Last Modified: Tue, 23 May 2023 23:16:52 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e3fa3ecf227f1ebec3c55bd0f33660f55a4c72c7c98126866fdb24c8eeb994`  
		Last Modified: Tue, 23 May 2023 23:17:32 GMT  
		Size: 47.3 MB (47282718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4a035c4ce960fbf0c1cc8f49f3ae3a551717a393f49d9816680b83232429f2`  
		Last Modified: Tue, 23 May 2023 23:17:25 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26.3` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:469c8395bc63238cbf8edbd03ee7fcfa1e612886983ae96ed3d01f5e2a161f63
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (134023049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3397e0751df6f6f99a3d83b78814985cdc24393e1908c11c7637c0600a5bec6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:01:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:32:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:32:06 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 18:32:17 GMT
ENV TELEGRAF_VERSION=1.26.3
# Tue, 13 Jun 2023 18:32:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Jun 2023 18:32:23 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Jun 2023 18:32:23 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Jun 2023 18:32:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 18:32:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751c9c60873892c6128382a04355bf76576dd23d87e5fdad03161dba5a2db45e`  
		Last Modified: Tue, 13 Jun 2023 03:08:33 GMT  
		Size: 15.7 MB (15746563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f7beb564cd4e17ac6f0066d8923c3e1a33cf5131542c873cd289e83bc2f98d`  
		Last Modified: Tue, 13 Jun 2023 18:32:50 GMT  
		Size: 18.6 MB (18598375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73606481ffac7e00171316db43e6998cf7b12ad1484bf62c4f7da607957b601`  
		Last Modified: Tue, 13 Jun 2023 18:32:47 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76673891e1d56c6ac4aeff9b37b2aba2292b7b4d707c24da4b6a620be7bf451c`  
		Last Modified: Tue, 13 Jun 2023 18:33:06 GMT  
		Size: 46.0 MB (45971825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780d64765ed31438940ad94e7d16ce89b012387a5f84b3b3650a8d7802125bd9`  
		Last Modified: Tue, 13 Jun 2023 18:33:01 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26.3-alpine`

```console
$ docker pull telegraf@sha256:bcc8de7293da7691bb01ae7d92d5028697c75326505ab952c77e3f30beb26e8f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.26.3-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:4355ab72932e3c3458f983d3f4ec18b038a0e6555bbac3b78a3bda15fe0b097b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.4 MB (56438425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e1ba951eb6880d6b98c3f0aace8c3d03eeb423de7ed6be2e5de4a913fe5e97a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Mar 2023 02:39:58 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 22 May 2023 21:20:15 GMT
ENV TELEGRAF_VERSION=1.26.3
# Mon, 22 May 2023 21:20:21 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 22 May 2023 21:20:21 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 22 May 2023 21:20:22 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 22 May 2023 21:20:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 22 May 2023 21:20:22 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc4e566a0dbfe02f4f43cee08d69aba4ae1fac7498203229b86614b5d893657`  
		Last Modified: Thu, 30 Mar 2023 02:40:39 GMT  
		Size: 2.7 MB (2671310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:840e49ac9f99eaec4020a3323146a8b2397c8db1cc172fa8a23508fa57667ba0`  
		Last Modified: Mon, 22 May 2023 21:21:03 GMT  
		Size: 50.4 MB (50391946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49481bb95fc2dde1fd38d56151df02d8be684e818fd3a2e72f65d5f274074515`  
		Last Modified: Mon, 22 May 2023 21:20:55 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26.3-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:dc6bfbc3c98a8b50f8da8f65fc86bb36a3dab1f5a1c35c0141a70476fab5351a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51778071 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80638ca136f6fff412e37d8a330474c503d0bfc1b1673bc77dbff94df832ca0c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:17:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Mar 2023 05:53:19 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 22 May 2023 20:51:12 GMT
ENV TELEGRAF_VERSION=1.26.3
# Mon, 22 May 2023 20:51:23 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 22 May 2023 20:51:24 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 22 May 2023 20:51:24 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 22 May 2023 20:51:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 22 May 2023 20:51:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed363db396bd455184362560a01cd691a111fe2dea827312e4f70ec9d621fee`  
		Last Modified: Thu, 30 Mar 2023 04:18:04 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667a1eb2ec7610bdd0add751f09715319b000a6f9d65d272224680b46dd4871b`  
		Last Modified: Thu, 30 Mar 2023 05:53:39 GMT  
		Size: 2.7 MB (2703331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6ef0ba6ccd8cc39ee7047af6650f38b324fc134cd9b5c857d116a923c039f2d`  
		Last Modified: Mon, 22 May 2023 20:51:56 GMT  
		Size: 45.8 MB (45812280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb87779c95194a7e41abdfa9ffbc2da15f428fd56b1f87f491da22256a4c57a0`  
		Last Modified: Mon, 22 May 2023 20:51:51 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.27`

```console
$ docker pull telegraf@sha256:9c46bf2b9eabe1db507b6ef99ddd19577ed64a746cd550dbaf5073ad57a11241
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.27` - linux; amd64

```console
$ docker pull telegraf@sha256:54f58415e414e57affc349ef4b62ca8c998571475d6b343bb1c68a5276677e9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.1 MB (143144537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c808179f1e9318d913634acbe9cfa7d0615525e4a8e2bdfc65a130b7fb96a14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 May 2023 01:20:00 GMT
ADD file:150a6453ab2258061c1a1549ab119df752bdc2c2c84028fa0e83a0663cd8cedf in / 
# Tue, 23 May 2023 01:20:01 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:48:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 20:36:19 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 20:36:21 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 12 Jun 2023 19:23:16 GMT
ENV TELEGRAF_VERSION=1.27.0
# Mon, 12 Jun 2023 19:23:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Mon, 12 Jun 2023 19:23:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 12 Jun 2023 19:23:22 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Mon, 12 Jun 2023 19:23:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Jun 2023 19:23:22 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:bd73737482dd5575526c7207872963479808d979ab2741c321706b8553918474`  
		Last Modified: Tue, 23 May 2023 01:23:46 GMT  
		Size: 55.0 MB (55049027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6710592d62aa1338ac1c1c363dedc255659f666cc41441c7e0f735c484db10ff`  
		Last Modified: Tue, 23 May 2023 01:56:06 GMT  
		Size: 15.8 MB (15760489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342d6d3ae9d9daf15efede898e8707fb9967951505106804ac53dd29f5e0f0ae`  
		Last Modified: Tue, 23 May 2023 20:36:59 GMT  
		Size: 18.8 MB (18759968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b674984b48670e73e773310e315a978db8ed074adccaff1f0152f6fa88914a43`  
		Last Modified: Tue, 23 May 2023 20:36:57 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0210ea2be0d97a6efdd13e85e544949654e0b94f1565c2326d9b8b1bdc972868`  
		Last Modified: Mon, 12 Jun 2023 19:23:58 GMT  
		Size: 53.6 MB (53572912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3cc0450f22544041e06662d208fea06e2027cc46bbae5483352c8c2c92fbb4`  
		Last Modified: Mon, 12 Jun 2023 19:23:49 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:ebb8eedc17d40eba47972a6fa26049b9443c2de34bf67f249fe799de1858e8e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.7 MB (132683761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:191c149d327519175115201e60c03b2a43ffaa6cfc8bc55f9bfb478ec611550f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 May 2023 00:57:45 GMT
ADD file:d8748d34e524d93a6df76d2a8ea8ca32ca04897521719f9f1f2a88ec692dd69e in / 
# Tue, 23 May 2023 00:57:45 GMT
CMD ["bash"]
# Tue, 23 May 2023 09:54:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 23:16:17 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 23:16:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 12 Jun 2023 20:14:08 GMT
ENV TELEGRAF_VERSION=1.27.0
# Mon, 12 Jun 2023 20:14:15 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Mon, 12 Jun 2023 20:14:16 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 12 Jun 2023 20:14:16 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Mon, 12 Jun 2023 20:14:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Jun 2023 20:14:16 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:29949e2d07dd1e283862cb4c3d4ec3043f1d54a1ac59f7b7a998ed9038a0243c`  
		Last Modified: Tue, 23 May 2023 01:01:23 GMT  
		Size: 50.2 MB (50210000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aaf40f65a7bdc041e615a5825b6ae62227f6a7ceec53af9e210fb62293e0bd2`  
		Last Modified: Tue, 23 May 2023 10:04:45 GMT  
		Size: 14.9 MB (14868582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fa44955cadb3e3d3d5fe86d27c4488b7e7aac3646248014cc6911ff7195039`  
		Last Modified: Tue, 23 May 2023 23:16:55 GMT  
		Size: 17.5 MB (17462338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e198f55fd4a95bb93ec5e99c99bf326613e1a6bad919dda290b804d7b627934`  
		Last Modified: Tue, 23 May 2023 23:16:52 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf35db1597432e97f40b5654396929e3122a11d7bb80f6f386019f84b8d3c17`  
		Last Modified: Mon, 12 Jun 2023 20:14:36 GMT  
		Size: 50.1 MB (50140690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789bf4d947e2c7713739b13712bddf384d8336e4e2380a55e6c572f8b6127a2a`  
		Last Modified: Mon, 12 Jun 2023 20:14:27 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:0a5b380d04db9ca43e02c93374ecc03fdc8cb8de54928522af3a276f0d005c80
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.8 MB (136782425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d46ddc43978731f3dbb7730d557d92847e6067918a6e9eec74f72207f71e61dc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:01:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:32:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:32:06 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 18:32:27 GMT
ENV TELEGRAF_VERSION=1.27.0
# Tue, 13 Jun 2023 18:32:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Jun 2023 18:32:31 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Jun 2023 18:32:31 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Jun 2023 18:32:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 18:32:31 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751c9c60873892c6128382a04355bf76576dd23d87e5fdad03161dba5a2db45e`  
		Last Modified: Tue, 13 Jun 2023 03:08:33 GMT  
		Size: 15.7 MB (15746563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f7beb564cd4e17ac6f0066d8923c3e1a33cf5131542c873cd289e83bc2f98d`  
		Last Modified: Tue, 13 Jun 2023 18:32:50 GMT  
		Size: 18.6 MB (18598375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73606481ffac7e00171316db43e6998cf7b12ad1484bf62c4f7da607957b601`  
		Last Modified: Tue, 13 Jun 2023 18:32:47 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b386b6ac686ceffe9ef1031e6d8cf8f8a986aa3abf49d85a719e50199947e7c5`  
		Last Modified: Tue, 13 Jun 2023 18:33:21 GMT  
		Size: 48.7 MB (48731199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79aaad56bf2200970306cd3a79d4a12bcd89d2b50edcf2f1ca2e761c800c2425`  
		Last Modified: Tue, 13 Jun 2023 18:33:16 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.27-alpine`

```console
$ docker pull telegraf@sha256:68ef9419df22292a9acbb89b39650d36c5e39a0272ac0f7c42706eef038f9fd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.27-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:a3245d3a0128cd96f5eea48ccdbd7b7e304a0d33883fcaa71d8269c3538a67f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59440594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e7958e377188f51d9cf9c6f231d65c63afd10d12b7783e952498dc8561d3ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Mar 2023 02:39:58 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 12 Jun 2023 19:23:25 GMT
ENV TELEGRAF_VERSION=1.27.0
# Mon, 12 Jun 2023 19:23:32 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 12 Jun 2023 19:23:32 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 12 Jun 2023 19:23:32 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 12 Jun 2023 19:23:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Jun 2023 19:23:32 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc4e566a0dbfe02f4f43cee08d69aba4ae1fac7498203229b86614b5d893657`  
		Last Modified: Thu, 30 Mar 2023 02:40:39 GMT  
		Size: 2.7 MB (2671310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f51bb152d58c88b0f815f199c5bdd92e9580ab075953d54b0333a69a3c43cf0`  
		Last Modified: Mon, 12 Jun 2023 19:24:16 GMT  
		Size: 53.4 MB (53394116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469b30fba184223e94fac64eaead6e3b60aadad0fe58231554f80430e6a6146e`  
		Last Modified: Mon, 12 Jun 2023 19:24:08 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:f4fbd8917e41abfa057e9899d9ecc6c7a206c083d397e90b9f5f8d228d3d4f8a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54528967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38af578ba18a572085fd9556a971efc545085ffdd9773a60b737c4dc7d5e699f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:17:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Mar 2023 05:53:19 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 12 Jun 2023 19:48:58 GMT
ENV TELEGRAF_VERSION=1.27.0
# Mon, 12 Jun 2023 19:49:05 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 12 Jun 2023 19:49:06 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 12 Jun 2023 19:49:06 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 12 Jun 2023 19:49:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Jun 2023 19:49:07 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed363db396bd455184362560a01cd691a111fe2dea827312e4f70ec9d621fee`  
		Last Modified: Thu, 30 Mar 2023 04:18:04 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667a1eb2ec7610bdd0add751f09715319b000a6f9d65d272224680b46dd4871b`  
		Last Modified: Thu, 30 Mar 2023 05:53:39 GMT  
		Size: 2.7 MB (2703331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46eacd3f9034d15fced4ab863cb6a50f6f36b32b8b72c70492c938265aea0543`  
		Last Modified: Mon, 12 Jun 2023 19:49:43 GMT  
		Size: 48.6 MB (48563175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aab598248a1189173eee42464c064e4c5d2471a618ca761b8502f9f09576f8a`  
		Last Modified: Mon, 12 Jun 2023 19:49:37 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.27.0`

```console
$ docker pull telegraf@sha256:9c46bf2b9eabe1db507b6ef99ddd19577ed64a746cd550dbaf5073ad57a11241
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.27.0` - linux; amd64

```console
$ docker pull telegraf@sha256:54f58415e414e57affc349ef4b62ca8c998571475d6b343bb1c68a5276677e9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.1 MB (143144537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c808179f1e9318d913634acbe9cfa7d0615525e4a8e2bdfc65a130b7fb96a14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 May 2023 01:20:00 GMT
ADD file:150a6453ab2258061c1a1549ab119df752bdc2c2c84028fa0e83a0663cd8cedf in / 
# Tue, 23 May 2023 01:20:01 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:48:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 20:36:19 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 20:36:21 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 12 Jun 2023 19:23:16 GMT
ENV TELEGRAF_VERSION=1.27.0
# Mon, 12 Jun 2023 19:23:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Mon, 12 Jun 2023 19:23:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 12 Jun 2023 19:23:22 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Mon, 12 Jun 2023 19:23:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Jun 2023 19:23:22 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:bd73737482dd5575526c7207872963479808d979ab2741c321706b8553918474`  
		Last Modified: Tue, 23 May 2023 01:23:46 GMT  
		Size: 55.0 MB (55049027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6710592d62aa1338ac1c1c363dedc255659f666cc41441c7e0f735c484db10ff`  
		Last Modified: Tue, 23 May 2023 01:56:06 GMT  
		Size: 15.8 MB (15760489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342d6d3ae9d9daf15efede898e8707fb9967951505106804ac53dd29f5e0f0ae`  
		Last Modified: Tue, 23 May 2023 20:36:59 GMT  
		Size: 18.8 MB (18759968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b674984b48670e73e773310e315a978db8ed074adccaff1f0152f6fa88914a43`  
		Last Modified: Tue, 23 May 2023 20:36:57 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0210ea2be0d97a6efdd13e85e544949654e0b94f1565c2326d9b8b1bdc972868`  
		Last Modified: Mon, 12 Jun 2023 19:23:58 GMT  
		Size: 53.6 MB (53572912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3cc0450f22544041e06662d208fea06e2027cc46bbae5483352c8c2c92fbb4`  
		Last Modified: Mon, 12 Jun 2023 19:23:49 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27.0` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:ebb8eedc17d40eba47972a6fa26049b9443c2de34bf67f249fe799de1858e8e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.7 MB (132683761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:191c149d327519175115201e60c03b2a43ffaa6cfc8bc55f9bfb478ec611550f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 May 2023 00:57:45 GMT
ADD file:d8748d34e524d93a6df76d2a8ea8ca32ca04897521719f9f1f2a88ec692dd69e in / 
# Tue, 23 May 2023 00:57:45 GMT
CMD ["bash"]
# Tue, 23 May 2023 09:54:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 23:16:17 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 23:16:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 12 Jun 2023 20:14:08 GMT
ENV TELEGRAF_VERSION=1.27.0
# Mon, 12 Jun 2023 20:14:15 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Mon, 12 Jun 2023 20:14:16 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 12 Jun 2023 20:14:16 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Mon, 12 Jun 2023 20:14:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Jun 2023 20:14:16 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:29949e2d07dd1e283862cb4c3d4ec3043f1d54a1ac59f7b7a998ed9038a0243c`  
		Last Modified: Tue, 23 May 2023 01:01:23 GMT  
		Size: 50.2 MB (50210000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aaf40f65a7bdc041e615a5825b6ae62227f6a7ceec53af9e210fb62293e0bd2`  
		Last Modified: Tue, 23 May 2023 10:04:45 GMT  
		Size: 14.9 MB (14868582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fa44955cadb3e3d3d5fe86d27c4488b7e7aac3646248014cc6911ff7195039`  
		Last Modified: Tue, 23 May 2023 23:16:55 GMT  
		Size: 17.5 MB (17462338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e198f55fd4a95bb93ec5e99c99bf326613e1a6bad919dda290b804d7b627934`  
		Last Modified: Tue, 23 May 2023 23:16:52 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf35db1597432e97f40b5654396929e3122a11d7bb80f6f386019f84b8d3c17`  
		Last Modified: Mon, 12 Jun 2023 20:14:36 GMT  
		Size: 50.1 MB (50140690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789bf4d947e2c7713739b13712bddf384d8336e4e2380a55e6c572f8b6127a2a`  
		Last Modified: Mon, 12 Jun 2023 20:14:27 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27.0` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:0a5b380d04db9ca43e02c93374ecc03fdc8cb8de54928522af3a276f0d005c80
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.8 MB (136782425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d46ddc43978731f3dbb7730d557d92847e6067918a6e9eec74f72207f71e61dc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:01:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:32:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:32:06 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 18:32:27 GMT
ENV TELEGRAF_VERSION=1.27.0
# Tue, 13 Jun 2023 18:32:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Jun 2023 18:32:31 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Jun 2023 18:32:31 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Jun 2023 18:32:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 18:32:31 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751c9c60873892c6128382a04355bf76576dd23d87e5fdad03161dba5a2db45e`  
		Last Modified: Tue, 13 Jun 2023 03:08:33 GMT  
		Size: 15.7 MB (15746563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f7beb564cd4e17ac6f0066d8923c3e1a33cf5131542c873cd289e83bc2f98d`  
		Last Modified: Tue, 13 Jun 2023 18:32:50 GMT  
		Size: 18.6 MB (18598375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73606481ffac7e00171316db43e6998cf7b12ad1484bf62c4f7da607957b601`  
		Last Modified: Tue, 13 Jun 2023 18:32:47 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b386b6ac686ceffe9ef1031e6d8cf8f8a986aa3abf49d85a719e50199947e7c5`  
		Last Modified: Tue, 13 Jun 2023 18:33:21 GMT  
		Size: 48.7 MB (48731199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79aaad56bf2200970306cd3a79d4a12bcd89d2b50edcf2f1ca2e761c800c2425`  
		Last Modified: Tue, 13 Jun 2023 18:33:16 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.27.0-alpine`

```console
$ docker pull telegraf@sha256:68ef9419df22292a9acbb89b39650d36c5e39a0272ac0f7c42706eef038f9fd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.27.0-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:a3245d3a0128cd96f5eea48ccdbd7b7e304a0d33883fcaa71d8269c3538a67f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59440594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e7958e377188f51d9cf9c6f231d65c63afd10d12b7783e952498dc8561d3ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Mar 2023 02:39:58 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 12 Jun 2023 19:23:25 GMT
ENV TELEGRAF_VERSION=1.27.0
# Mon, 12 Jun 2023 19:23:32 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 12 Jun 2023 19:23:32 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 12 Jun 2023 19:23:32 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 12 Jun 2023 19:23:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Jun 2023 19:23:32 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc4e566a0dbfe02f4f43cee08d69aba4ae1fac7498203229b86614b5d893657`  
		Last Modified: Thu, 30 Mar 2023 02:40:39 GMT  
		Size: 2.7 MB (2671310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f51bb152d58c88b0f815f199c5bdd92e9580ab075953d54b0333a69a3c43cf0`  
		Last Modified: Mon, 12 Jun 2023 19:24:16 GMT  
		Size: 53.4 MB (53394116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469b30fba184223e94fac64eaead6e3b60aadad0fe58231554f80430e6a6146e`  
		Last Modified: Mon, 12 Jun 2023 19:24:08 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27.0-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:f4fbd8917e41abfa057e9899d9ecc6c7a206c083d397e90b9f5f8d228d3d4f8a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54528967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38af578ba18a572085fd9556a971efc545085ffdd9773a60b737c4dc7d5e699f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:17:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Mar 2023 05:53:19 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 12 Jun 2023 19:48:58 GMT
ENV TELEGRAF_VERSION=1.27.0
# Mon, 12 Jun 2023 19:49:05 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 12 Jun 2023 19:49:06 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 12 Jun 2023 19:49:06 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 12 Jun 2023 19:49:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Jun 2023 19:49:07 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed363db396bd455184362560a01cd691a111fe2dea827312e4f70ec9d621fee`  
		Last Modified: Thu, 30 Mar 2023 04:18:04 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667a1eb2ec7610bdd0add751f09715319b000a6f9d65d272224680b46dd4871b`  
		Last Modified: Thu, 30 Mar 2023 05:53:39 GMT  
		Size: 2.7 MB (2703331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46eacd3f9034d15fced4ab863cb6a50f6f36b32b8b72c70492c938265aea0543`  
		Last Modified: Mon, 12 Jun 2023 19:49:43 GMT  
		Size: 48.6 MB (48563175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aab598248a1189173eee42464c064e4c5d2471a618ca761b8502f9f09576f8a`  
		Last Modified: Mon, 12 Jun 2023 19:49:37 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:68ef9419df22292a9acbb89b39650d36c5e39a0272ac0f7c42706eef038f9fd8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:a3245d3a0128cd96f5eea48ccdbd7b7e304a0d33883fcaa71d8269c3538a67f8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.4 MB (59440594 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e7958e377188f51d9cf9c6f231d65c63afd10d12b7783e952498dc8561d3ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:46:49 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Mar 2023 02:39:58 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 12 Jun 2023 19:23:25 GMT
ENV TELEGRAF_VERSION=1.27.0
# Mon, 12 Jun 2023 19:23:32 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 12 Jun 2023 19:23:32 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 12 Jun 2023 19:23:32 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 12 Jun 2023 19:23:32 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Jun 2023 19:23:32 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347b672f7645299da052e0672f5ba2941477e3da3a3f4b2b3af29c9bd761da80`  
		Last Modified: Wed, 29 Mar 2023 19:47:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dc4e566a0dbfe02f4f43cee08d69aba4ae1fac7498203229b86614b5d893657`  
		Last Modified: Thu, 30 Mar 2023 02:40:39 GMT  
		Size: 2.7 MB (2671310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f51bb152d58c88b0f815f199c5bdd92e9580ab075953d54b0333a69a3c43cf0`  
		Last Modified: Mon, 12 Jun 2023 19:24:16 GMT  
		Size: 53.4 MB (53394116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469b30fba184223e94fac64eaead6e3b60aadad0fe58231554f80430e6a6146e`  
		Last Modified: Mon, 12 Jun 2023 19:24:08 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:f4fbd8917e41abfa057e9899d9ecc6c7a206c083d397e90b9f5f8d228d3d4f8a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54528967 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38af578ba18a572085fd9556a971efc545085ffdd9773a60b737c4dc7d5e699f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 04:17:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 30 Mar 2023 05:53:19 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 12 Jun 2023 19:48:58 GMT
ENV TELEGRAF_VERSION=1.27.0
# Mon, 12 Jun 2023 19:49:05 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 12 Jun 2023 19:49:06 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 12 Jun 2023 19:49:06 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 12 Jun 2023 19:49:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Jun 2023 19:49:07 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed363db396bd455184362560a01cd691a111fe2dea827312e4f70ec9d621fee`  
		Last Modified: Thu, 30 Mar 2023 04:18:04 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667a1eb2ec7610bdd0add751f09715319b000a6f9d65d272224680b46dd4871b`  
		Last Modified: Thu, 30 Mar 2023 05:53:39 GMT  
		Size: 2.7 MB (2703331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46eacd3f9034d15fced4ab863cb6a50f6f36b32b8b72c70492c938265aea0543`  
		Last Modified: Mon, 12 Jun 2023 19:49:43 GMT  
		Size: 48.6 MB (48563175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aab598248a1189173eee42464c064e4c5d2471a618ca761b8502f9f09576f8a`  
		Last Modified: Mon, 12 Jun 2023 19:49:37 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:9c46bf2b9eabe1db507b6ef99ddd19577ed64a746cd550dbaf5073ad57a11241
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:54f58415e414e57affc349ef4b62ca8c998571475d6b343bb1c68a5276677e9c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.1 MB (143144537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c808179f1e9318d913634acbe9cfa7d0615525e4a8e2bdfc65a130b7fb96a14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 May 2023 01:20:00 GMT
ADD file:150a6453ab2258061c1a1549ab119df752bdc2c2c84028fa0e83a0663cd8cedf in / 
# Tue, 23 May 2023 01:20:01 GMT
CMD ["bash"]
# Tue, 23 May 2023 01:48:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 20:36:19 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 20:36:21 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 12 Jun 2023 19:23:16 GMT
ENV TELEGRAF_VERSION=1.27.0
# Mon, 12 Jun 2023 19:23:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Mon, 12 Jun 2023 19:23:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 12 Jun 2023 19:23:22 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Mon, 12 Jun 2023 19:23:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Jun 2023 19:23:22 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:bd73737482dd5575526c7207872963479808d979ab2741c321706b8553918474`  
		Last Modified: Tue, 23 May 2023 01:23:46 GMT  
		Size: 55.0 MB (55049027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6710592d62aa1338ac1c1c363dedc255659f666cc41441c7e0f735c484db10ff`  
		Last Modified: Tue, 23 May 2023 01:56:06 GMT  
		Size: 15.8 MB (15760489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:342d6d3ae9d9daf15efede898e8707fb9967951505106804ac53dd29f5e0f0ae`  
		Last Modified: Tue, 23 May 2023 20:36:59 GMT  
		Size: 18.8 MB (18759968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b674984b48670e73e773310e315a978db8ed074adccaff1f0152f6fa88914a43`  
		Last Modified: Tue, 23 May 2023 20:36:57 GMT  
		Size: 1.8 KB (1796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0210ea2be0d97a6efdd13e85e544949654e0b94f1565c2326d9b8b1bdc972868`  
		Last Modified: Mon, 12 Jun 2023 19:23:58 GMT  
		Size: 53.6 MB (53572912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3cc0450f22544041e06662d208fea06e2027cc46bbae5483352c8c2c92fbb4`  
		Last Modified: Mon, 12 Jun 2023 19:23:49 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:ebb8eedc17d40eba47972a6fa26049b9443c2de34bf67f249fe799de1858e8e4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.7 MB (132683761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:191c149d327519175115201e60c03b2a43ffaa6cfc8bc55f9bfb478ec611550f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 May 2023 00:57:45 GMT
ADD file:d8748d34e524d93a6df76d2a8ea8ca32ca04897521719f9f1f2a88ec692dd69e in / 
# Tue, 23 May 2023 00:57:45 GMT
CMD ["bash"]
# Tue, 23 May 2023 09:54:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 23:16:17 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 May 2023 23:16:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 12 Jun 2023 20:14:08 GMT
ENV TELEGRAF_VERSION=1.27.0
# Mon, 12 Jun 2023 20:14:15 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Mon, 12 Jun 2023 20:14:16 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 12 Jun 2023 20:14:16 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Mon, 12 Jun 2023 20:14:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 12 Jun 2023 20:14:16 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:29949e2d07dd1e283862cb4c3d4ec3043f1d54a1ac59f7b7a998ed9038a0243c`  
		Last Modified: Tue, 23 May 2023 01:01:23 GMT  
		Size: 50.2 MB (50210000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aaf40f65a7bdc041e615a5825b6ae62227f6a7ceec53af9e210fb62293e0bd2`  
		Last Modified: Tue, 23 May 2023 10:04:45 GMT  
		Size: 14.9 MB (14868582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91fa44955cadb3e3d3d5fe86d27c4488b7e7aac3646248014cc6911ff7195039`  
		Last Modified: Tue, 23 May 2023 23:16:55 GMT  
		Size: 17.5 MB (17462338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e198f55fd4a95bb93ec5e99c99bf326613e1a6bad919dda290b804d7b627934`  
		Last Modified: Tue, 23 May 2023 23:16:52 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf35db1597432e97f40b5654396929e3122a11d7bb80f6f386019f84b8d3c17`  
		Last Modified: Mon, 12 Jun 2023 20:14:36 GMT  
		Size: 50.1 MB (50140690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789bf4d947e2c7713739b13712bddf384d8336e4e2380a55e6c572f8b6127a2a`  
		Last Modified: Mon, 12 Jun 2023 20:14:27 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:0a5b380d04db9ca43e02c93374ecc03fdc8cb8de54928522af3a276f0d005c80
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.8 MB (136782425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d46ddc43978731f3dbb7730d557d92847e6067918a6e9eec74f72207f71e61dc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 12 Jun 2023 23:40:22 GMT
ADD file:caddd2f40296ec5c1bf7487617ca8694cfff9a1d9b7484159e203b6514cb5f5f in / 
# Mon, 12 Jun 2023 23:40:23 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:01:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:32:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:32:06 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 18:32:27 GMT
ENV TELEGRAF_VERSION=1.27.0
# Tue, 13 Jun 2023 18:32:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Jun 2023 18:32:31 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Jun 2023 18:32:31 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Jun 2023 18:32:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 18:32:31 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:663ccfaf62a5d7b997bca03d1dc6d5dfff01b9e0de08d86dbea8957ea92d7d16`  
		Last Modified: Mon, 12 Jun 2023 23:44:25 GMT  
		Size: 53.7 MB (53704136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751c9c60873892c6128382a04355bf76576dd23d87e5fdad03161dba5a2db45e`  
		Last Modified: Tue, 13 Jun 2023 03:08:33 GMT  
		Size: 15.7 MB (15746563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f7beb564cd4e17ac6f0066d8923c3e1a33cf5131542c873cd289e83bc2f98d`  
		Last Modified: Tue, 13 Jun 2023 18:32:50 GMT  
		Size: 18.6 MB (18598375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a73606481ffac7e00171316db43e6998cf7b12ad1484bf62c4f7da607957b601`  
		Last Modified: Tue, 13 Jun 2023 18:32:47 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b386b6ac686ceffe9ef1031e6d8cf8f8a986aa3abf49d85a719e50199947e7c5`  
		Last Modified: Tue, 13 Jun 2023 18:33:21 GMT  
		Size: 48.7 MB (48731199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79aaad56bf2200970306cd3a79d4a12bcd89d2b50edcf2f1ca2e761c800c2425`  
		Last Modified: Tue, 13 Jun 2023 18:33:16 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
