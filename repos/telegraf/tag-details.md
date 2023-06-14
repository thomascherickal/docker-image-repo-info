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
$ docker pull telegraf@sha256:a05ecc44f138547620d37244042992832e1a0be8b9a76911751b60c95d0222d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.25` - linux; amd64

```console
$ docker pull telegraf@sha256:e86c416c14f06caddc86432e90450a7c62c93484af7ccf89da05b5d96e5bff32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.2 MB (136154409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9886a81f0da476902b5154185ce2750fd23306cc7546919841130eebc171c2ec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 19:52:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 19:52:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 19:52:59 GMT
ENV TELEGRAF_VERSION=1.25.3
# Tue, 13 Jun 2023 19:53:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Jun 2023 19:53:04 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Jun 2023 19:53:04 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Jun 2023 19:53:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 19:53:04 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87e6f3487e1d7e61ee7a415e0ced4eb6f0b3484eb1e15a4339d110d3cadf899`  
		Last Modified: Tue, 13 Jun 2023 03:37:33 GMT  
		Size: 15.8 MB (15760332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a1bd817f4c2f4115a0999d4f802752e4012c281b24cb70d83cfe54ae359eae`  
		Last Modified: Tue, 13 Jun 2023 19:53:43 GMT  
		Size: 18.8 MB (18760197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e8cc37fc85816666c16f78e6251af17182a69419caf030788879fe7a9880e2`  
		Last Modified: Tue, 13 Jun 2023 19:53:39 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55eae750f94d68c5689853cd9e9c3ea297662ccde52336f0a258cc33f1212956`  
		Last Modified: Tue, 13 Jun 2023 19:53:47 GMT  
		Size: 46.6 MB (46576569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf0ce674b272be783b900c4d531f59c913a40328825cb2d466677ab01727f3e`  
		Last Modified: Tue, 13 Jun 2023 19:53:39 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:7be9ddb2ab7c0b6ce3c8ecc5004bbf48578691a7796c4d30f569e440b9674359
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125935103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2be66a15408e43b073dbe24052b270e2c64ae84060e2e97f9348897b25947bee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:34 GMT
ADD file:6edc8f94d2ebc83d6081e1c4567963d0060a842c767eaff959a6e5c6d09247b5 in / 
# Mon, 12 Jun 2023 23:58:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:55:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 00:44:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 00:44:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 14 Jun 2023 00:44:58 GMT
ENV TELEGRAF_VERSION=1.25.3
# Wed, 14 Jun 2023 00:45:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 14 Jun 2023 00:45:05 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 14 Jun 2023 00:45:05 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 14 Jun 2023 00:45:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 00:45:05 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:23807bbf2a5fd14b7975a9e82f4a5530bbba520f31b382cc4b4ce2e77e075ace`  
		Last Modified: Tue, 13 Jun 2023 00:04:02 GMT  
		Size: 50.2 MB (50218141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3330bf88d2bbd0baa313813532130c140958ecb30e8bdd1d1a990d63261a23`  
		Last Modified: Tue, 13 Jun 2023 05:03:43 GMT  
		Size: 14.9 MB (14868599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f16447055228f0130c57f508a98b44ac4ac5f32ae194f1c0c816da8a0529d1`  
		Last Modified: Wed, 14 Jun 2023 00:45:39 GMT  
		Size: 17.5 MB (17462264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c8cb983fff2ba7e59511794ebeabf104d7b9bac5ead1141d66e87f91eec6a3`  
		Last Modified: Wed, 14 Jun 2023 00:45:36 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8c3a75655f9234cf0bd8cf732aa332f0f07b87f45ba180b0c0be80947cb0ac`  
		Last Modified: Wed, 14 Jun 2023 00:45:44 GMT  
		Size: 43.4 MB (43383948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbbdc224b8c4949989583a2fbad866afb34267156c25cec0b4a855f93e99f4a`  
		Last Modified: Wed, 14 Jun 2023 00:45:36 GMT  
		Size: 343.0 B  
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
$ docker pull telegraf@sha256:a05ecc44f138547620d37244042992832e1a0be8b9a76911751b60c95d0222d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.25.3` - linux; amd64

```console
$ docker pull telegraf@sha256:e86c416c14f06caddc86432e90450a7c62c93484af7ccf89da05b5d96e5bff32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.2 MB (136154409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9886a81f0da476902b5154185ce2750fd23306cc7546919841130eebc171c2ec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 19:52:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 19:52:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 19:52:59 GMT
ENV TELEGRAF_VERSION=1.25.3
# Tue, 13 Jun 2023 19:53:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Jun 2023 19:53:04 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Jun 2023 19:53:04 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Jun 2023 19:53:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 19:53:04 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87e6f3487e1d7e61ee7a415e0ced4eb6f0b3484eb1e15a4339d110d3cadf899`  
		Last Modified: Tue, 13 Jun 2023 03:37:33 GMT  
		Size: 15.8 MB (15760332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a1bd817f4c2f4115a0999d4f802752e4012c281b24cb70d83cfe54ae359eae`  
		Last Modified: Tue, 13 Jun 2023 19:53:43 GMT  
		Size: 18.8 MB (18760197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e8cc37fc85816666c16f78e6251af17182a69419caf030788879fe7a9880e2`  
		Last Modified: Tue, 13 Jun 2023 19:53:39 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55eae750f94d68c5689853cd9e9c3ea297662ccde52336f0a258cc33f1212956`  
		Last Modified: Tue, 13 Jun 2023 19:53:47 GMT  
		Size: 46.6 MB (46576569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf0ce674b272be783b900c4d531f59c913a40328825cb2d466677ab01727f3e`  
		Last Modified: Tue, 13 Jun 2023 19:53:39 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25.3` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:7be9ddb2ab7c0b6ce3c8ecc5004bbf48578691a7796c4d30f569e440b9674359
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125935103 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2be66a15408e43b073dbe24052b270e2c64ae84060e2e97f9348897b25947bee`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:34 GMT
ADD file:6edc8f94d2ebc83d6081e1c4567963d0060a842c767eaff959a6e5c6d09247b5 in / 
# Mon, 12 Jun 2023 23:58:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:55:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 00:44:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 00:44:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 14 Jun 2023 00:44:58 GMT
ENV TELEGRAF_VERSION=1.25.3
# Wed, 14 Jun 2023 00:45:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 14 Jun 2023 00:45:05 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 14 Jun 2023 00:45:05 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 14 Jun 2023 00:45:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 00:45:05 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:23807bbf2a5fd14b7975a9e82f4a5530bbba520f31b382cc4b4ce2e77e075ace`  
		Last Modified: Tue, 13 Jun 2023 00:04:02 GMT  
		Size: 50.2 MB (50218141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3330bf88d2bbd0baa313813532130c140958ecb30e8bdd1d1a990d63261a23`  
		Last Modified: Tue, 13 Jun 2023 05:03:43 GMT  
		Size: 14.9 MB (14868599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f16447055228f0130c57f508a98b44ac4ac5f32ae194f1c0c816da8a0529d1`  
		Last Modified: Wed, 14 Jun 2023 00:45:39 GMT  
		Size: 17.5 MB (17462264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c8cb983fff2ba7e59511794ebeabf104d7b9bac5ead1141d66e87f91eec6a3`  
		Last Modified: Wed, 14 Jun 2023 00:45:36 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8c3a75655f9234cf0bd8cf732aa332f0f07b87f45ba180b0c0be80947cb0ac`  
		Last Modified: Wed, 14 Jun 2023 00:45:44 GMT  
		Size: 43.4 MB (43383948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbbdc224b8c4949989583a2fbad866afb34267156c25cec0b4a855f93e99f4a`  
		Last Modified: Wed, 14 Jun 2023 00:45:36 GMT  
		Size: 343.0 B  
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
$ docker pull telegraf@sha256:9ae65425ecf22b27be6e3d504b6ad591c8c1f14bbb7587a244f7ee1fe398f8da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.26` - linux; amd64

```console
$ docker pull telegraf@sha256:b271df59fe08617a0598eff088662b59981159ec61ca0dad8f3f964513c234ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140130353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e66ca0bc680780f4b5a9d32e254b4cf43fac184a8afad191df553b6cc9c9ec4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 19:52:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 19:52:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 19:53:08 GMT
ENV TELEGRAF_VERSION=1.26.3
# Tue, 13 Jun 2023 19:53:13 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Jun 2023 19:53:14 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Jun 2023 19:53:14 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Jun 2023 19:53:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 19:53:14 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87e6f3487e1d7e61ee7a415e0ced4eb6f0b3484eb1e15a4339d110d3cadf899`  
		Last Modified: Tue, 13 Jun 2023 03:37:33 GMT  
		Size: 15.8 MB (15760332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a1bd817f4c2f4115a0999d4f802752e4012c281b24cb70d83cfe54ae359eae`  
		Last Modified: Tue, 13 Jun 2023 19:53:43 GMT  
		Size: 18.8 MB (18760197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e8cc37fc85816666c16f78e6251af17182a69419caf030788879fe7a9880e2`  
		Last Modified: Tue, 13 Jun 2023 19:53:39 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5e2332dc39583e500e170a6d351643573579abbb1c3af1e7b9208f1163ba5c`  
		Last Modified: Tue, 13 Jun 2023 19:54:03 GMT  
		Size: 50.6 MB (50552512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd201639d4d6c9104ce4cb41e94334f1500f94ef37336919358a4ed7318e434`  
		Last Modified: Tue, 13 Jun 2023 19:53:55 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:883cab3b832531cca6036c99d9422740e40d1b959822ec5ed6ebf4f0c7c9739d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129833865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70fe971ffb2955b251ab25956ed7d15f156cc601cb2fd5d59136d151db6883f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:34 GMT
ADD file:6edc8f94d2ebc83d6081e1c4567963d0060a842c767eaff959a6e5c6d09247b5 in / 
# Mon, 12 Jun 2023 23:58:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:55:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 00:44:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 00:44:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 14 Jun 2023 00:45:07 GMT
ENV TELEGRAF_VERSION=1.26.3
# Wed, 14 Jun 2023 00:45:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 14 Jun 2023 00:45:15 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 14 Jun 2023 00:45:15 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 14 Jun 2023 00:45:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 00:45:15 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:23807bbf2a5fd14b7975a9e82f4a5530bbba520f31b382cc4b4ce2e77e075ace`  
		Last Modified: Tue, 13 Jun 2023 00:04:02 GMT  
		Size: 50.2 MB (50218141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3330bf88d2bbd0baa313813532130c140958ecb30e8bdd1d1a990d63261a23`  
		Last Modified: Tue, 13 Jun 2023 05:03:43 GMT  
		Size: 14.9 MB (14868599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f16447055228f0130c57f508a98b44ac4ac5f32ae194f1c0c816da8a0529d1`  
		Last Modified: Wed, 14 Jun 2023 00:45:39 GMT  
		Size: 17.5 MB (17462264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c8cb983fff2ba7e59511794ebeabf104d7b9bac5ead1141d66e87f91eec6a3`  
		Last Modified: Wed, 14 Jun 2023 00:45:36 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c91bea7408f85e6c4fee89bb0e62f3f3e6ac0fb43082630a8b59fc226095a9`  
		Last Modified: Wed, 14 Jun 2023 00:46:00 GMT  
		Size: 47.3 MB (47282708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b07ccbcc04b29debd973b65a5fbed3acf9189119f8a96c23a288a8448d4377e`  
		Last Modified: Wed, 14 Jun 2023 00:45:52 GMT  
		Size: 345.0 B  
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
$ docker pull telegraf@sha256:9ae65425ecf22b27be6e3d504b6ad591c8c1f14bbb7587a244f7ee1fe398f8da
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.26.3` - linux; amd64

```console
$ docker pull telegraf@sha256:b271df59fe08617a0598eff088662b59981159ec61ca0dad8f3f964513c234ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140130353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e66ca0bc680780f4b5a9d32e254b4cf43fac184a8afad191df553b6cc9c9ec4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 19:52:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 19:52:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 19:53:08 GMT
ENV TELEGRAF_VERSION=1.26.3
# Tue, 13 Jun 2023 19:53:13 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Jun 2023 19:53:14 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Jun 2023 19:53:14 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Jun 2023 19:53:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 19:53:14 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87e6f3487e1d7e61ee7a415e0ced4eb6f0b3484eb1e15a4339d110d3cadf899`  
		Last Modified: Tue, 13 Jun 2023 03:37:33 GMT  
		Size: 15.8 MB (15760332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a1bd817f4c2f4115a0999d4f802752e4012c281b24cb70d83cfe54ae359eae`  
		Last Modified: Tue, 13 Jun 2023 19:53:43 GMT  
		Size: 18.8 MB (18760197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e8cc37fc85816666c16f78e6251af17182a69419caf030788879fe7a9880e2`  
		Last Modified: Tue, 13 Jun 2023 19:53:39 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f5e2332dc39583e500e170a6d351643573579abbb1c3af1e7b9208f1163ba5c`  
		Last Modified: Tue, 13 Jun 2023 19:54:03 GMT  
		Size: 50.6 MB (50552512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebd201639d4d6c9104ce4cb41e94334f1500f94ef37336919358a4ed7318e434`  
		Last Modified: Tue, 13 Jun 2023 19:53:55 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26.3` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:883cab3b832531cca6036c99d9422740e40d1b959822ec5ed6ebf4f0c7c9739d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129833865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70fe971ffb2955b251ab25956ed7d15f156cc601cb2fd5d59136d151db6883f5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:34 GMT
ADD file:6edc8f94d2ebc83d6081e1c4567963d0060a842c767eaff959a6e5c6d09247b5 in / 
# Mon, 12 Jun 2023 23:58:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:55:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 00:44:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 00:44:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 14 Jun 2023 00:45:07 GMT
ENV TELEGRAF_VERSION=1.26.3
# Wed, 14 Jun 2023 00:45:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 14 Jun 2023 00:45:15 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 14 Jun 2023 00:45:15 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 14 Jun 2023 00:45:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 00:45:15 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:23807bbf2a5fd14b7975a9e82f4a5530bbba520f31b382cc4b4ce2e77e075ace`  
		Last Modified: Tue, 13 Jun 2023 00:04:02 GMT  
		Size: 50.2 MB (50218141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3330bf88d2bbd0baa313813532130c140958ecb30e8bdd1d1a990d63261a23`  
		Last Modified: Tue, 13 Jun 2023 05:03:43 GMT  
		Size: 14.9 MB (14868599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f16447055228f0130c57f508a98b44ac4ac5f32ae194f1c0c816da8a0529d1`  
		Last Modified: Wed, 14 Jun 2023 00:45:39 GMT  
		Size: 17.5 MB (17462264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c8cb983fff2ba7e59511794ebeabf104d7b9bac5ead1141d66e87f91eec6a3`  
		Last Modified: Wed, 14 Jun 2023 00:45:36 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c91bea7408f85e6c4fee89bb0e62f3f3e6ac0fb43082630a8b59fc226095a9`  
		Last Modified: Wed, 14 Jun 2023 00:46:00 GMT  
		Size: 47.3 MB (47282708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b07ccbcc04b29debd973b65a5fbed3acf9189119f8a96c23a288a8448d4377e`  
		Last Modified: Wed, 14 Jun 2023 00:45:52 GMT  
		Size: 345.0 B  
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
$ docker pull telegraf@sha256:76175ba6f3e25db7757c80a5d165e4dddf1069e08d8226e9535bdb464068be65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.27` - linux; amd64

```console
$ docker pull telegraf@sha256:6d309ce4ec0c722688638a32fddc67fdb7ea6e387d22a22d5b0c96eea565a6e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.2 MB (143150759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:245ed83f748572e64d13c688a308dc0974fe6ed0f5f7c82f9c05b4cab67a6bc8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 19:52:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 19:52:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 19:53:19 GMT
ENV TELEGRAF_VERSION=1.27.0
# Tue, 13 Jun 2023 19:53:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Jun 2023 19:53:24 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Jun 2023 19:53:24 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Jun 2023 19:53:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 19:53:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87e6f3487e1d7e61ee7a415e0ced4eb6f0b3484eb1e15a4339d110d3cadf899`  
		Last Modified: Tue, 13 Jun 2023 03:37:33 GMT  
		Size: 15.8 MB (15760332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a1bd817f4c2f4115a0999d4f802752e4012c281b24cb70d83cfe54ae359eae`  
		Last Modified: Tue, 13 Jun 2023 19:53:43 GMT  
		Size: 18.8 MB (18760197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e8cc37fc85816666c16f78e6251af17182a69419caf030788879fe7a9880e2`  
		Last Modified: Tue, 13 Jun 2023 19:53:39 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d7f8aeba4eca40e57044bd41a26d2581d5a39c201dcbf489d069dd3bd14c2f`  
		Last Modified: Tue, 13 Jun 2023 19:54:20 GMT  
		Size: 53.6 MB (53572918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9263108d6f4924541d80366aae40641cca1b2542ea12df478ba470193dcd1e28`  
		Last Modified: Tue, 13 Jun 2023 19:54:12 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:fb467058cfc2a6694d32e59d2678d34f9cc968679e98688ca2671336d90f467a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.7 MB (132691805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fe3aafb2d52e3d696cd382630f477bc1b099684eb9fb138fed825dfd8ec3ccd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:34 GMT
ADD file:6edc8f94d2ebc83d6081e1c4567963d0060a842c767eaff959a6e5c6d09247b5 in / 
# Mon, 12 Jun 2023 23:58:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:55:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 00:44:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 00:44:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 14 Jun 2023 00:45:17 GMT
ENV TELEGRAF_VERSION=1.27.0
# Wed, 14 Jun 2023 00:45:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 14 Jun 2023 00:45:24 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 14 Jun 2023 00:45:24 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 14 Jun 2023 00:45:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 00:45:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:23807bbf2a5fd14b7975a9e82f4a5530bbba520f31b382cc4b4ce2e77e075ace`  
		Last Modified: Tue, 13 Jun 2023 00:04:02 GMT  
		Size: 50.2 MB (50218141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3330bf88d2bbd0baa313813532130c140958ecb30e8bdd1d1a990d63261a23`  
		Last Modified: Tue, 13 Jun 2023 05:03:43 GMT  
		Size: 14.9 MB (14868599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f16447055228f0130c57f508a98b44ac4ac5f32ae194f1c0c816da8a0529d1`  
		Last Modified: Wed, 14 Jun 2023 00:45:39 GMT  
		Size: 17.5 MB (17462264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c8cb983fff2ba7e59511794ebeabf104d7b9bac5ead1141d66e87f91eec6a3`  
		Last Modified: Wed, 14 Jun 2023 00:45:36 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1145d87ff2b62a0ab8f9edad3525e9446fd7ae1a475970b948f2b2ed1c39aca`  
		Last Modified: Wed, 14 Jun 2023 00:46:16 GMT  
		Size: 50.1 MB (50140650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b6450a307c04abdb396b10bea56fdd0ec9558c8d3c8e3f5eabdf3877606465`  
		Last Modified: Wed, 14 Jun 2023 00:46:08 GMT  
		Size: 343.0 B  
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
$ docker pull telegraf@sha256:76175ba6f3e25db7757c80a5d165e4dddf1069e08d8226e9535bdb464068be65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.27.0` - linux; amd64

```console
$ docker pull telegraf@sha256:6d309ce4ec0c722688638a32fddc67fdb7ea6e387d22a22d5b0c96eea565a6e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.2 MB (143150759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:245ed83f748572e64d13c688a308dc0974fe6ed0f5f7c82f9c05b4cab67a6bc8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 19:52:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 19:52:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 19:53:19 GMT
ENV TELEGRAF_VERSION=1.27.0
# Tue, 13 Jun 2023 19:53:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Jun 2023 19:53:24 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Jun 2023 19:53:24 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Jun 2023 19:53:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 19:53:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87e6f3487e1d7e61ee7a415e0ced4eb6f0b3484eb1e15a4339d110d3cadf899`  
		Last Modified: Tue, 13 Jun 2023 03:37:33 GMT  
		Size: 15.8 MB (15760332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a1bd817f4c2f4115a0999d4f802752e4012c281b24cb70d83cfe54ae359eae`  
		Last Modified: Tue, 13 Jun 2023 19:53:43 GMT  
		Size: 18.8 MB (18760197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e8cc37fc85816666c16f78e6251af17182a69419caf030788879fe7a9880e2`  
		Last Modified: Tue, 13 Jun 2023 19:53:39 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d7f8aeba4eca40e57044bd41a26d2581d5a39c201dcbf489d069dd3bd14c2f`  
		Last Modified: Tue, 13 Jun 2023 19:54:20 GMT  
		Size: 53.6 MB (53572918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9263108d6f4924541d80366aae40641cca1b2542ea12df478ba470193dcd1e28`  
		Last Modified: Tue, 13 Jun 2023 19:54:12 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27.0` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:fb467058cfc2a6694d32e59d2678d34f9cc968679e98688ca2671336d90f467a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.7 MB (132691805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fe3aafb2d52e3d696cd382630f477bc1b099684eb9fb138fed825dfd8ec3ccd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:34 GMT
ADD file:6edc8f94d2ebc83d6081e1c4567963d0060a842c767eaff959a6e5c6d09247b5 in / 
# Mon, 12 Jun 2023 23:58:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:55:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 00:44:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 00:44:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 14 Jun 2023 00:45:17 GMT
ENV TELEGRAF_VERSION=1.27.0
# Wed, 14 Jun 2023 00:45:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 14 Jun 2023 00:45:24 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 14 Jun 2023 00:45:24 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 14 Jun 2023 00:45:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 00:45:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:23807bbf2a5fd14b7975a9e82f4a5530bbba520f31b382cc4b4ce2e77e075ace`  
		Last Modified: Tue, 13 Jun 2023 00:04:02 GMT  
		Size: 50.2 MB (50218141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3330bf88d2bbd0baa313813532130c140958ecb30e8bdd1d1a990d63261a23`  
		Last Modified: Tue, 13 Jun 2023 05:03:43 GMT  
		Size: 14.9 MB (14868599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f16447055228f0130c57f508a98b44ac4ac5f32ae194f1c0c816da8a0529d1`  
		Last Modified: Wed, 14 Jun 2023 00:45:39 GMT  
		Size: 17.5 MB (17462264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c8cb983fff2ba7e59511794ebeabf104d7b9bac5ead1141d66e87f91eec6a3`  
		Last Modified: Wed, 14 Jun 2023 00:45:36 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1145d87ff2b62a0ab8f9edad3525e9446fd7ae1a475970b948f2b2ed1c39aca`  
		Last Modified: Wed, 14 Jun 2023 00:46:16 GMT  
		Size: 50.1 MB (50140650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b6450a307c04abdb396b10bea56fdd0ec9558c8d3c8e3f5eabdf3877606465`  
		Last Modified: Wed, 14 Jun 2023 00:46:08 GMT  
		Size: 343.0 B  
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
$ docker pull telegraf@sha256:76175ba6f3e25db7757c80a5d165e4dddf1069e08d8226e9535bdb464068be65
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:6d309ce4ec0c722688638a32fddc67fdb7ea6e387d22a22d5b0c96eea565a6e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.2 MB (143150759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:245ed83f748572e64d13c688a308dc0974fe6ed0f5f7c82f9c05b4cab67a6bc8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 12 Jun 2023 23:20:54 GMT
ADD file:e530b0563ea53d97b2f28e62149a665900196f86611df99a88c7a8ab2097b95d in / 
# Mon, 12 Jun 2023 23:20:54 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:29:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 19:52:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 19:52:59 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 13 Jun 2023 19:53:19 GMT
ENV TELEGRAF_VERSION=1.27.0
# Tue, 13 Jun 2023 19:53:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 13 Jun 2023 19:53:24 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 13 Jun 2023 19:53:24 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 13 Jun 2023 19:53:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 13 Jun 2023 19:53:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:93c2d578e4211e82e47e7ada9ed05d1869a2362c6f7509f2ee8d91ccebfb7fbd`  
		Last Modified: Mon, 12 Jun 2023 23:26:08 GMT  
		Size: 55.1 MB (55055162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c87e6f3487e1d7e61ee7a415e0ced4eb6f0b3484eb1e15a4339d110d3cadf899`  
		Last Modified: Tue, 13 Jun 2023 03:37:33 GMT  
		Size: 15.8 MB (15760332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a1bd817f4c2f4115a0999d4f802752e4012c281b24cb70d83cfe54ae359eae`  
		Last Modified: Tue, 13 Jun 2023 19:53:43 GMT  
		Size: 18.8 MB (18760197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e8cc37fc85816666c16f78e6251af17182a69419caf030788879fe7a9880e2`  
		Last Modified: Tue, 13 Jun 2023 19:53:39 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d7f8aeba4eca40e57044bd41a26d2581d5a39c201dcbf489d069dd3bd14c2f`  
		Last Modified: Tue, 13 Jun 2023 19:54:20 GMT  
		Size: 53.6 MB (53572918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9263108d6f4924541d80366aae40641cca1b2542ea12df478ba470193dcd1e28`  
		Last Modified: Tue, 13 Jun 2023 19:54:12 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:fb467058cfc2a6694d32e59d2678d34f9cc968679e98688ca2671336d90f467a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.7 MB (132691805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fe3aafb2d52e3d696cd382630f477bc1b099684eb9fb138fed825dfd8ec3ccd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 12 Jun 2023 23:58:34 GMT
ADD file:6edc8f94d2ebc83d6081e1c4567963d0060a842c767eaff959a6e5c6d09247b5 in / 
# Mon, 12 Jun 2023 23:58:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 04:55:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 00:44:57 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 14 Jun 2023 00:44:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 14 Jun 2023 00:45:17 GMT
ENV TELEGRAF_VERSION=1.27.0
# Wed, 14 Jun 2023 00:45:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 14 Jun 2023 00:45:24 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 14 Jun 2023 00:45:24 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 14 Jun 2023 00:45:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Jun 2023 00:45:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:23807bbf2a5fd14b7975a9e82f4a5530bbba520f31b382cc4b4ce2e77e075ace`  
		Last Modified: Tue, 13 Jun 2023 00:04:02 GMT  
		Size: 50.2 MB (50218141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3330bf88d2bbd0baa313813532130c140958ecb30e8bdd1d1a990d63261a23`  
		Last Modified: Tue, 13 Jun 2023 05:03:43 GMT  
		Size: 14.9 MB (14868599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f16447055228f0130c57f508a98b44ac4ac5f32ae194f1c0c816da8a0529d1`  
		Last Modified: Wed, 14 Jun 2023 00:45:39 GMT  
		Size: 17.5 MB (17462264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c8cb983fff2ba7e59511794ebeabf104d7b9bac5ead1141d66e87f91eec6a3`  
		Last Modified: Wed, 14 Jun 2023 00:45:36 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1145d87ff2b62a0ab8f9edad3525e9446fd7ae1a475970b948f2b2ed1c39aca`  
		Last Modified: Wed, 14 Jun 2023 00:46:16 GMT  
		Size: 50.1 MB (50140650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b6450a307c04abdb396b10bea56fdd0ec9558c8d3c8e3f5eabdf3877606465`  
		Last Modified: Wed, 14 Jun 2023 00:46:08 GMT  
		Size: 343.0 B  
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
