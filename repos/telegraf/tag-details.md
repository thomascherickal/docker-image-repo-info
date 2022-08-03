<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `telegraf`

-	[`telegraf:1.21`](#telegraf121)
-	[`telegraf:1.21-alpine`](#telegraf121-alpine)
-	[`telegraf:1.21.4`](#telegraf1214)
-	[`telegraf:1.21.4-alpine`](#telegraf1214-alpine)
-	[`telegraf:1.22`](#telegraf122)
-	[`telegraf:1.22-alpine`](#telegraf122-alpine)
-	[`telegraf:1.22.4`](#telegraf1224)
-	[`telegraf:1.22.4-alpine`](#telegraf1224-alpine)
-	[`telegraf:1.23`](#telegraf123)
-	[`telegraf:1.23-alpine`](#telegraf123-alpine)
-	[`telegraf:1.23.3`](#telegraf1233)
-	[`telegraf:1.23.3-alpine`](#telegraf1233-alpine)
-	[`telegraf:alpine`](#telegrafalpine)
-	[`telegraf:latest`](#telegraflatest)

## `telegraf:1.21`

```console
$ docker pull telegraf@sha256:dddf18d06c382ff00e033361df4ac08eecff59b83a78e3675e0c71fff39ac0a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.21` - linux; amd64

```console
$ docker pull telegraf@sha256:5f46aa78e7525faba64b2c9259b03c1df0cb1a0e9f180522862964853d340ee1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127452909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ae0a94f516312d6061d542fc64f627483c4550e5bb54670d87fe371cf59bfa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 02 Aug 2022 01:19:54 GMT
ADD file:d0f758e50c654c225f6c7f03e8a579efc9106437051573bdbae5e63b1c4b2c1f in / 
# Tue, 02 Aug 2022 01:19:54 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:46:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:47:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 03 Aug 2022 02:19:18 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 02:19:20 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 Aug 2022 02:19:20 GMT
ENV TELEGRAF_VERSION=1.21.4
# Wed, 03 Aug 2022 02:19:24 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 Aug 2022 02:19:24 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 Aug 2022 02:19:24 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 Aug 2022 02:19:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 Aug 2022 02:19:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:001c52e26ad57e3b25b439ee0052f6692e5c0f2d5d982a00a8819ace5e521452`  
		Last Modified: Tue, 02 Aug 2022 01:23:44 GMT  
		Size: 55.0 MB (54999331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d4b9b6e964657da49910b495173d6c4f0d9bc47b3b44273cf82fd32723d165`  
		Last Modified: Tue, 02 Aug 2022 02:18:26 GMT  
		Size: 5.2 MB (5156256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2068746827ec1b043b571e4788693eab7e9b2a95301176512791f8c317a2816a`  
		Last Modified: Tue, 02 Aug 2022 02:18:26 GMT  
		Size: 10.9 MB (10876485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fa4837c01bf0ec37537e86b40953e1be0c5a2f73ab15bb8d9267c641f2937c`  
		Last Modified: Wed, 03 Aug 2022 02:20:07 GMT  
		Size: 18.8 MB (18760336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78684b72b16c9b01fb02bc8c8f26552e94b5655a2a12226c010bc75c8dd0a514`  
		Last Modified: Wed, 03 Aug 2022 02:20:04 GMT  
		Size: 2.9 KB (2902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9777ab61f64d50cb13f1c34982bcf6315ff858bf890e1f4a32a68edc1aa01a`  
		Last Modified: Wed, 03 Aug 2022 02:20:11 GMT  
		Size: 37.7 MB (37657257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481a3b2147e96488e42ba1ab58537b033fac1924de70e60512574c6b5f504dd8`  
		Last Modified: Wed, 03 Aug 2022 02:20:04 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.21` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:50ff3272770937bd0838348a37ab032d7f98548406ebae9b07a74f876904e156
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117733735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14b44304e22e65c0820904b7d760ff3b22835d8db79c1164bccf1f49adcbac37`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:16 GMT
ADD file:72ef8362158fcd45f10c6fa2dc3ea411e81f700ecb92faf37cb6dc1887756f9d in / 
# Tue, 12 Jul 2022 00:59:17 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 13:25:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 13:26:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Jul 2022 21:45:39 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2022 21:45:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 29 Jul 2022 21:45:41 GMT
ENV TELEGRAF_VERSION=1.21.4
# Fri, 29 Jul 2022 21:45:46 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 29 Jul 2022 21:45:46 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 29 Jul 2022 21:45:46 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 29 Jul 2022 21:45:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Jul 2022 21:45:46 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a8a55ed160b9a554de2e46b828d606a0829d8d9f19c79bc47eddac683aeb2b91`  
		Last Modified: Tue, 12 Jul 2022 01:11:51 GMT  
		Size: 50.2 MB (50194881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de0d7ddb0c03f1180487d49fda757592276a2a2eedc3f36d7bd625e1de85cc4`  
		Last Modified: Thu, 28 Jul 2022 13:52:28 GMT  
		Size: 4.9 MB (4924805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc57b4c2f87bc9e41a073ca20fcc00a5105e1147f67f5968e36f843fff2da78a`  
		Last Modified: Thu, 28 Jul 2022 13:52:29 GMT  
		Size: 10.2 MB (10218017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801295d59b33e19109e93ada5f5bd22493781b3b4427766642f38297fd9a394f`  
		Last Modified: Fri, 29 Jul 2022 21:46:40 GMT  
		Size: 17.5 MB (17462132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281582a6a59d8bf62488abef853dd03ba854dcd8e11e36253bdacbbb59a16d7a`  
		Last Modified: Fri, 29 Jul 2022 21:46:36 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0623c936a59a33faec380f23773d86bfae4abe4b750f8c330b4fe60dd853a84c`  
		Last Modified: Fri, 29 Jul 2022 21:46:43 GMT  
		Size: 34.9 MB (34930671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c41ea2b8e1d6c2bdb18c0e5808ec3093b9c0c088b5cb33a15d6be2d91729ad`  
		Last Modified: Fri, 29 Jul 2022 21:46:36 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.21` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:af11dfaaae2d8465eee7ed5eda21c9b281af358e7b0ec7802fdf30443717f2b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122035689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b48e9ba64535319459c4693ed716dc1709d104b1f44cbf3a86a29e97f0a4049`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:24 GMT
ADD file:5972a7ce0f1d89d63e5ed48011838c998fa506cd34f8e5f0b0070039cd74c5b9 in / 
# Tue, 02 Aug 2022 00:40:25 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:24:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:24:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 22:58:27 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 22:58:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 02 Aug 2022 22:58:30 GMT
ENV TELEGRAF_VERSION=1.21.4
# Tue, 02 Aug 2022 22:58:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 02 Aug 2022 22:58:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 02 Aug 2022 22:58:37 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 02 Aug 2022 22:58:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 Aug 2022 22:58:38 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:114ba63dd73a866ac1bb59fe594dfd218f44ac9b4fa4b2c68499da5584fcfa9d`  
		Last Modified: Tue, 02 Aug 2022 00:45:33 GMT  
		Size: 53.7 MB (53683005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0b8a8acead4d7bf71c232054b2a0a8e08eb3e1e2cf46f9f3dba68723e88c85`  
		Last Modified: Tue, 02 Aug 2022 01:44:32 GMT  
		Size: 5.1 MB (5148901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ea641ee67989acdb6af3d8b9b984ecd751a2a83c3b7ce071542b31c9ac1304`  
		Last Modified: Tue, 02 Aug 2022 01:44:33 GMT  
		Size: 10.7 MB (10657494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b22bb61739a9b58a9acd5e791a783e60521e183266080deabfebd494ebb04a`  
		Last Modified: Tue, 02 Aug 2022 22:59:29 GMT  
		Size: 18.4 MB (18382753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7992c681678681934e95ece4d739305c6598ac402216ea7726cbdc2e2f758516`  
		Last Modified: Tue, 02 Aug 2022 22:59:26 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f18af010b88df3f42b274ff1b90f5ee5cbe6a9edb1b72268d92dc9fc43c8930`  
		Last Modified: Tue, 02 Aug 2022 22:59:32 GMT  
		Size: 34.2 MB (34160332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4075fdb52c959f8234b2c7261ccdf536a4bbdb29c43ff0b669f16943d674dff0`  
		Last Modified: Tue, 02 Aug 2022 22:59:26 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.21-alpine`

```console
$ docker pull telegraf@sha256:9075e180705041df3bee8e648d870e569f50583bf390c17e9ab9ffad4aae0060
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.21-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:2153f289617aec080afc5e5e6402068649ff0d4cf26ca4a4994b37a6f9f2b6c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43686262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23daa1ecb777459f77d7aab6bb64a46c89004f0dfad4663a9dade41a4fb49df7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 02:25:55 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 20 Jul 2022 02:25:58 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 20 Jul 2022 02:25:58 GMT
ENV TELEGRAF_VERSION=1.21.4
# Wed, 20 Jul 2022 02:26:04 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 20 Jul 2022 02:26:04 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 20 Jul 2022 02:26:04 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 20 Jul 2022 02:26:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Jul 2022 02:26:04 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1d6c3bdc90884e20be4b8964afbc50fc83dac03969c542117bb4c4e59802fb`  
		Last Modified: Wed, 20 Jul 2022 02:26:48 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7afda0100e244bcaa7520aff1df3205abf84be1593c127ee83151d1395be22`  
		Last Modified: Wed, 20 Jul 2022 02:26:49 GMT  
		Size: 3.4 MB (3372891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9555aad715806c0fea6ee0e9cf31acc2f7fb1c9067f0c5ef2ca4ff54b43f7838`  
		Last Modified: Wed, 20 Jul 2022 02:26:55 GMT  
		Size: 37.5 MB (37498245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:272fc0e7895dc73648dc5d5d2a639de3f70ed4c044ad8e49ea25773172a8c329`  
		Last Modified: Wed, 20 Jul 2022 02:26:48 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.21.4`

```console
$ docker pull telegraf@sha256:dddf18d06c382ff00e033361df4ac08eecff59b83a78e3675e0c71fff39ac0a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.21.4` - linux; amd64

```console
$ docker pull telegraf@sha256:5f46aa78e7525faba64b2c9259b03c1df0cb1a0e9f180522862964853d340ee1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127452909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ae0a94f516312d6061d542fc64f627483c4550e5bb54670d87fe371cf59bfa`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 02 Aug 2022 01:19:54 GMT
ADD file:d0f758e50c654c225f6c7f03e8a579efc9106437051573bdbae5e63b1c4b2c1f in / 
# Tue, 02 Aug 2022 01:19:54 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:46:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:47:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 03 Aug 2022 02:19:18 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 02:19:20 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 Aug 2022 02:19:20 GMT
ENV TELEGRAF_VERSION=1.21.4
# Wed, 03 Aug 2022 02:19:24 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 Aug 2022 02:19:24 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 Aug 2022 02:19:24 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 Aug 2022 02:19:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 Aug 2022 02:19:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:001c52e26ad57e3b25b439ee0052f6692e5c0f2d5d982a00a8819ace5e521452`  
		Last Modified: Tue, 02 Aug 2022 01:23:44 GMT  
		Size: 55.0 MB (54999331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d4b9b6e964657da49910b495173d6c4f0d9bc47b3b44273cf82fd32723d165`  
		Last Modified: Tue, 02 Aug 2022 02:18:26 GMT  
		Size: 5.2 MB (5156256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2068746827ec1b043b571e4788693eab7e9b2a95301176512791f8c317a2816a`  
		Last Modified: Tue, 02 Aug 2022 02:18:26 GMT  
		Size: 10.9 MB (10876485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fa4837c01bf0ec37537e86b40953e1be0c5a2f73ab15bb8d9267c641f2937c`  
		Last Modified: Wed, 03 Aug 2022 02:20:07 GMT  
		Size: 18.8 MB (18760336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78684b72b16c9b01fb02bc8c8f26552e94b5655a2a12226c010bc75c8dd0a514`  
		Last Modified: Wed, 03 Aug 2022 02:20:04 GMT  
		Size: 2.9 KB (2902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df9777ab61f64d50cb13f1c34982bcf6315ff858bf890e1f4a32a68edc1aa01a`  
		Last Modified: Wed, 03 Aug 2022 02:20:11 GMT  
		Size: 37.7 MB (37657257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481a3b2147e96488e42ba1ab58537b033fac1924de70e60512574c6b5f504dd8`  
		Last Modified: Wed, 03 Aug 2022 02:20:04 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.21.4` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:50ff3272770937bd0838348a37ab032d7f98548406ebae9b07a74f876904e156
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117733735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14b44304e22e65c0820904b7d760ff3b22835d8db79c1164bccf1f49adcbac37`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:16 GMT
ADD file:72ef8362158fcd45f10c6fa2dc3ea411e81f700ecb92faf37cb6dc1887756f9d in / 
# Tue, 12 Jul 2022 00:59:17 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 13:25:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 13:26:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Jul 2022 21:45:39 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2022 21:45:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 29 Jul 2022 21:45:41 GMT
ENV TELEGRAF_VERSION=1.21.4
# Fri, 29 Jul 2022 21:45:46 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 29 Jul 2022 21:45:46 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 29 Jul 2022 21:45:46 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 29 Jul 2022 21:45:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Jul 2022 21:45:46 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a8a55ed160b9a554de2e46b828d606a0829d8d9f19c79bc47eddac683aeb2b91`  
		Last Modified: Tue, 12 Jul 2022 01:11:51 GMT  
		Size: 50.2 MB (50194881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de0d7ddb0c03f1180487d49fda757592276a2a2eedc3f36d7bd625e1de85cc4`  
		Last Modified: Thu, 28 Jul 2022 13:52:28 GMT  
		Size: 4.9 MB (4924805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc57b4c2f87bc9e41a073ca20fcc00a5105e1147f67f5968e36f843fff2da78a`  
		Last Modified: Thu, 28 Jul 2022 13:52:29 GMT  
		Size: 10.2 MB (10218017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801295d59b33e19109e93ada5f5bd22493781b3b4427766642f38297fd9a394f`  
		Last Modified: Fri, 29 Jul 2022 21:46:40 GMT  
		Size: 17.5 MB (17462132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281582a6a59d8bf62488abef853dd03ba854dcd8e11e36253bdacbbb59a16d7a`  
		Last Modified: Fri, 29 Jul 2022 21:46:36 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0623c936a59a33faec380f23773d86bfae4abe4b750f8c330b4fe60dd853a84c`  
		Last Modified: Fri, 29 Jul 2022 21:46:43 GMT  
		Size: 34.9 MB (34930671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72c41ea2b8e1d6c2bdb18c0e5808ec3093b9c0c088b5cb33a15d6be2d91729ad`  
		Last Modified: Fri, 29 Jul 2022 21:46:36 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.21.4` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:af11dfaaae2d8465eee7ed5eda21c9b281af358e7b0ec7802fdf30443717f2b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122035689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b48e9ba64535319459c4693ed716dc1709d104b1f44cbf3a86a29e97f0a4049`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:24 GMT
ADD file:5972a7ce0f1d89d63e5ed48011838c998fa506cd34f8e5f0b0070039cd74c5b9 in / 
# Tue, 02 Aug 2022 00:40:25 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:24:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:24:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 22:58:27 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 22:58:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 02 Aug 2022 22:58:30 GMT
ENV TELEGRAF_VERSION=1.21.4
# Tue, 02 Aug 2022 22:58:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 02 Aug 2022 22:58:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 02 Aug 2022 22:58:37 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 02 Aug 2022 22:58:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 Aug 2022 22:58:38 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:114ba63dd73a866ac1bb59fe594dfd218f44ac9b4fa4b2c68499da5584fcfa9d`  
		Last Modified: Tue, 02 Aug 2022 00:45:33 GMT  
		Size: 53.7 MB (53683005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0b8a8acead4d7bf71c232054b2a0a8e08eb3e1e2cf46f9f3dba68723e88c85`  
		Last Modified: Tue, 02 Aug 2022 01:44:32 GMT  
		Size: 5.1 MB (5148901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ea641ee67989acdb6af3d8b9b984ecd751a2a83c3b7ce071542b31c9ac1304`  
		Last Modified: Tue, 02 Aug 2022 01:44:33 GMT  
		Size: 10.7 MB (10657494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b22bb61739a9b58a9acd5e791a783e60521e183266080deabfebd494ebb04a`  
		Last Modified: Tue, 02 Aug 2022 22:59:29 GMT  
		Size: 18.4 MB (18382753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7992c681678681934e95ece4d739305c6598ac402216ea7726cbdc2e2f758516`  
		Last Modified: Tue, 02 Aug 2022 22:59:26 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f18af010b88df3f42b274ff1b90f5ee5cbe6a9edb1b72268d92dc9fc43c8930`  
		Last Modified: Tue, 02 Aug 2022 22:59:32 GMT  
		Size: 34.2 MB (34160332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4075fdb52c959f8234b2c7261ccdf536a4bbdb29c43ff0b669f16943d674dff0`  
		Last Modified: Tue, 02 Aug 2022 22:59:26 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.21.4-alpine`

```console
$ docker pull telegraf@sha256:9075e180705041df3bee8e648d870e569f50583bf390c17e9ab9ffad4aae0060
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.21.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:2153f289617aec080afc5e5e6402068649ff0d4cf26ca4a4994b37a6f9f2b6c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43686262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23daa1ecb777459f77d7aab6bb64a46c89004f0dfad4663a9dade41a4fb49df7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 02:25:55 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 20 Jul 2022 02:25:58 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 20 Jul 2022 02:25:58 GMT
ENV TELEGRAF_VERSION=1.21.4
# Wed, 20 Jul 2022 02:26:04 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 20 Jul 2022 02:26:04 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 20 Jul 2022 02:26:04 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 20 Jul 2022 02:26:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Jul 2022 02:26:04 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1d6c3bdc90884e20be4b8964afbc50fc83dac03969c542117bb4c4e59802fb`  
		Last Modified: Wed, 20 Jul 2022 02:26:48 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7afda0100e244bcaa7520aff1df3205abf84be1593c127ee83151d1395be22`  
		Last Modified: Wed, 20 Jul 2022 02:26:49 GMT  
		Size: 3.4 MB (3372891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9555aad715806c0fea6ee0e9cf31acc2f7fb1c9067f0c5ef2ca4ff54b43f7838`  
		Last Modified: Wed, 20 Jul 2022 02:26:55 GMT  
		Size: 37.5 MB (37498245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:272fc0e7895dc73648dc5d5d2a639de3f70ed4c044ad8e49ea25773172a8c329`  
		Last Modified: Wed, 20 Jul 2022 02:26:48 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.22`

```console
$ docker pull telegraf@sha256:7da40a458695cccb4de9367558d1d3cc9684f4039c8eb5d7811675f4939b9670
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.22` - linux; amd64

```console
$ docker pull telegraf@sha256:fc2d6b0853c3622a5292fc1655568e922d4ec6f37d2f6151c6fc4b5574a1a03c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.3 MB (130294429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8176d57ed66e2a89312bb48c54b5078600022105ba397e3b6febe13d76ae600f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 02 Aug 2022 01:19:54 GMT
ADD file:d0f758e50c654c225f6c7f03e8a579efc9106437051573bdbae5e63b1c4b2c1f in / 
# Tue, 02 Aug 2022 01:19:54 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:46:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:47:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 03 Aug 2022 02:19:18 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 02:19:20 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 Aug 2022 02:19:30 GMT
ENV TELEGRAF_VERSION=1.22.4
# Wed, 03 Aug 2022 02:19:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 Aug 2022 02:19:34 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 Aug 2022 02:19:34 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 Aug 2022 02:19:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 Aug 2022 02:19:34 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:001c52e26ad57e3b25b439ee0052f6692e5c0f2d5d982a00a8819ace5e521452`  
		Last Modified: Tue, 02 Aug 2022 01:23:44 GMT  
		Size: 55.0 MB (54999331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d4b9b6e964657da49910b495173d6c4f0d9bc47b3b44273cf82fd32723d165`  
		Last Modified: Tue, 02 Aug 2022 02:18:26 GMT  
		Size: 5.2 MB (5156256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2068746827ec1b043b571e4788693eab7e9b2a95301176512791f8c317a2816a`  
		Last Modified: Tue, 02 Aug 2022 02:18:26 GMT  
		Size: 10.9 MB (10876485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fa4837c01bf0ec37537e86b40953e1be0c5a2f73ab15bb8d9267c641f2937c`  
		Last Modified: Wed, 03 Aug 2022 02:20:07 GMT  
		Size: 18.8 MB (18760336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78684b72b16c9b01fb02bc8c8f26552e94b5655a2a12226c010bc75c8dd0a514`  
		Last Modified: Wed, 03 Aug 2022 02:20:04 GMT  
		Size: 2.9 KB (2902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a11d8034f36edb4e16ce28f2152d6fec1032048501d369b8a38613234ae402`  
		Last Modified: Wed, 03 Aug 2022 02:20:28 GMT  
		Size: 40.5 MB (40498777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566b0e6792138e76d830edec541ba25b0abc7a6b510ed7ca49f1f7768e20075c`  
		Last Modified: Wed, 03 Aug 2022 02:20:21 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.22` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:28e029735eb1d48fddd09798ddb24a528ddc326abab3a93a59699332d58f8a32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.7 MB (120724746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a241aa7de4af76f770a1fad25e5718582a6740e244cfadb7a414eed1cc3dfc7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:16 GMT
ADD file:72ef8362158fcd45f10c6fa2dc3ea411e81f700ecb92faf37cb6dc1887756f9d in / 
# Tue, 12 Jul 2022 00:59:17 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 13:25:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 13:26:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Jul 2022 21:45:39 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2022 21:45:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 29 Jul 2022 21:45:53 GMT
ENV TELEGRAF_VERSION=1.22.4
# Fri, 29 Jul 2022 21:45:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 29 Jul 2022 21:45:59 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 29 Jul 2022 21:45:59 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 29 Jul 2022 21:45:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Jul 2022 21:45:59 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a8a55ed160b9a554de2e46b828d606a0829d8d9f19c79bc47eddac683aeb2b91`  
		Last Modified: Tue, 12 Jul 2022 01:11:51 GMT  
		Size: 50.2 MB (50194881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de0d7ddb0c03f1180487d49fda757592276a2a2eedc3f36d7bd625e1de85cc4`  
		Last Modified: Thu, 28 Jul 2022 13:52:28 GMT  
		Size: 4.9 MB (4924805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc57b4c2f87bc9e41a073ca20fcc00a5105e1147f67f5968e36f843fff2da78a`  
		Last Modified: Thu, 28 Jul 2022 13:52:29 GMT  
		Size: 10.2 MB (10218017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801295d59b33e19109e93ada5f5bd22493781b3b4427766642f38297fd9a394f`  
		Last Modified: Fri, 29 Jul 2022 21:46:40 GMT  
		Size: 17.5 MB (17462132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281582a6a59d8bf62488abef853dd03ba854dcd8e11e36253bdacbbb59a16d7a`  
		Last Modified: Fri, 29 Jul 2022 21:46:36 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9124a342e40a4f75161fc22c685fb34f809d40655e6101d9916aa7dc23cc7831`  
		Last Modified: Fri, 29 Jul 2022 21:47:01 GMT  
		Size: 37.9 MB (37921681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eda0d8e6413bd60164de91e7ccaafb374de56761659d815d697fc383909cd2a`  
		Last Modified: Fri, 29 Jul 2022 21:46:54 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.22` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:a0b83997ae451a71613dc728fdf1dd9518707c62b01eb2d4754d48812f8f7000
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124686348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97bde2495b78fced58e8c1cba9862d4d0e9c08a803de66d5e938a829a26e184e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:24 GMT
ADD file:5972a7ce0f1d89d63e5ed48011838c998fa506cd34f8e5f0b0070039cd74c5b9 in / 
# Tue, 02 Aug 2022 00:40:25 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:24:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:24:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 22:58:27 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 22:58:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 02 Aug 2022 22:58:43 GMT
ENV TELEGRAF_VERSION=1.22.4
# Tue, 02 Aug 2022 22:58:48 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 02 Aug 2022 22:58:49 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 02 Aug 2022 22:58:50 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 02 Aug 2022 22:58:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 Aug 2022 22:58:51 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:114ba63dd73a866ac1bb59fe594dfd218f44ac9b4fa4b2c68499da5584fcfa9d`  
		Last Modified: Tue, 02 Aug 2022 00:45:33 GMT  
		Size: 53.7 MB (53683005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0b8a8acead4d7bf71c232054b2a0a8e08eb3e1e2cf46f9f3dba68723e88c85`  
		Last Modified: Tue, 02 Aug 2022 01:44:32 GMT  
		Size: 5.1 MB (5148901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ea641ee67989acdb6af3d8b9b984ecd751a2a83c3b7ce071542b31c9ac1304`  
		Last Modified: Tue, 02 Aug 2022 01:44:33 GMT  
		Size: 10.7 MB (10657494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b22bb61739a9b58a9acd5e791a783e60521e183266080deabfebd494ebb04a`  
		Last Modified: Tue, 02 Aug 2022 22:59:29 GMT  
		Size: 18.4 MB (18382753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7992c681678681934e95ece4d739305c6598ac402216ea7726cbdc2e2f758516`  
		Last Modified: Tue, 02 Aug 2022 22:59:26 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5787a3b346b420e74710d87245793734fd3277af3ec6274a2f4e8ad5f0183e9`  
		Last Modified: Tue, 02 Aug 2022 22:59:49 GMT  
		Size: 36.8 MB (36810994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be79842777b5861a646af4982b864132e2f8752e8bee0675d882ed12853fd202`  
		Last Modified: Tue, 02 Aug 2022 22:59:43 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.22-alpine`

```console
$ docker pull telegraf@sha256:bf27934d3967ab34011854e1951b00cd30218ff49d5e30512dada3a568782606
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.22-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:c9c0e1f082fc573fb815361cce09bdd05f4756ba427d445b3a3a9a6c060239fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46542137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9d178f642164168fecf5d636292cca6a61d896c8723830cf3717c3f3fd992c9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 02:25:55 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 20 Jul 2022 02:25:58 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 20 Jul 2022 02:26:08 GMT
ENV TELEGRAF_VERSION=1.22.4
# Wed, 20 Jul 2022 02:26:15 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 20 Jul 2022 02:26:15 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 20 Jul 2022 02:26:15 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 20 Jul 2022 02:26:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Jul 2022 02:26:15 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1d6c3bdc90884e20be4b8964afbc50fc83dac03969c542117bb4c4e59802fb`  
		Last Modified: Wed, 20 Jul 2022 02:26:48 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7afda0100e244bcaa7520aff1df3205abf84be1593c127ee83151d1395be22`  
		Last Modified: Wed, 20 Jul 2022 02:26:49 GMT  
		Size: 3.4 MB (3372891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1744c6d7f1d3b0cfc79904e1d04f119570f1aa76386244b2a87426468fd4d500`  
		Last Modified: Wed, 20 Jul 2022 02:27:11 GMT  
		Size: 40.4 MB (40354121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702b42dd6a8e2c24a184819f51f5ba8fa12e92b225839733cc72571c871ba5a1`  
		Last Modified: Wed, 20 Jul 2022 02:27:05 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.22.4`

```console
$ docker pull telegraf@sha256:7da40a458695cccb4de9367558d1d3cc9684f4039c8eb5d7811675f4939b9670
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.22.4` - linux; amd64

```console
$ docker pull telegraf@sha256:fc2d6b0853c3622a5292fc1655568e922d4ec6f37d2f6151c6fc4b5574a1a03c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.3 MB (130294429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8176d57ed66e2a89312bb48c54b5078600022105ba397e3b6febe13d76ae600f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 02 Aug 2022 01:19:54 GMT
ADD file:d0f758e50c654c225f6c7f03e8a579efc9106437051573bdbae5e63b1c4b2c1f in / 
# Tue, 02 Aug 2022 01:19:54 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:46:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:47:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 03 Aug 2022 02:19:18 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 02:19:20 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 Aug 2022 02:19:30 GMT
ENV TELEGRAF_VERSION=1.22.4
# Wed, 03 Aug 2022 02:19:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 Aug 2022 02:19:34 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 Aug 2022 02:19:34 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 Aug 2022 02:19:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 Aug 2022 02:19:34 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:001c52e26ad57e3b25b439ee0052f6692e5c0f2d5d982a00a8819ace5e521452`  
		Last Modified: Tue, 02 Aug 2022 01:23:44 GMT  
		Size: 55.0 MB (54999331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d4b9b6e964657da49910b495173d6c4f0d9bc47b3b44273cf82fd32723d165`  
		Last Modified: Tue, 02 Aug 2022 02:18:26 GMT  
		Size: 5.2 MB (5156256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2068746827ec1b043b571e4788693eab7e9b2a95301176512791f8c317a2816a`  
		Last Modified: Tue, 02 Aug 2022 02:18:26 GMT  
		Size: 10.9 MB (10876485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fa4837c01bf0ec37537e86b40953e1be0c5a2f73ab15bb8d9267c641f2937c`  
		Last Modified: Wed, 03 Aug 2022 02:20:07 GMT  
		Size: 18.8 MB (18760336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78684b72b16c9b01fb02bc8c8f26552e94b5655a2a12226c010bc75c8dd0a514`  
		Last Modified: Wed, 03 Aug 2022 02:20:04 GMT  
		Size: 2.9 KB (2902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a11d8034f36edb4e16ce28f2152d6fec1032048501d369b8a38613234ae402`  
		Last Modified: Wed, 03 Aug 2022 02:20:28 GMT  
		Size: 40.5 MB (40498777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:566b0e6792138e76d830edec541ba25b0abc7a6b510ed7ca49f1f7768e20075c`  
		Last Modified: Wed, 03 Aug 2022 02:20:21 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.22.4` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:28e029735eb1d48fddd09798ddb24a528ddc326abab3a93a59699332d58f8a32
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.7 MB (120724746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a241aa7de4af76f770a1fad25e5718582a6740e244cfadb7a414eed1cc3dfc7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:16 GMT
ADD file:72ef8362158fcd45f10c6fa2dc3ea411e81f700ecb92faf37cb6dc1887756f9d in / 
# Tue, 12 Jul 2022 00:59:17 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 13:25:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 13:26:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Jul 2022 21:45:39 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2022 21:45:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 29 Jul 2022 21:45:53 GMT
ENV TELEGRAF_VERSION=1.22.4
# Fri, 29 Jul 2022 21:45:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 29 Jul 2022 21:45:59 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 29 Jul 2022 21:45:59 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 29 Jul 2022 21:45:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Jul 2022 21:45:59 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a8a55ed160b9a554de2e46b828d606a0829d8d9f19c79bc47eddac683aeb2b91`  
		Last Modified: Tue, 12 Jul 2022 01:11:51 GMT  
		Size: 50.2 MB (50194881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de0d7ddb0c03f1180487d49fda757592276a2a2eedc3f36d7bd625e1de85cc4`  
		Last Modified: Thu, 28 Jul 2022 13:52:28 GMT  
		Size: 4.9 MB (4924805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc57b4c2f87bc9e41a073ca20fcc00a5105e1147f67f5968e36f843fff2da78a`  
		Last Modified: Thu, 28 Jul 2022 13:52:29 GMT  
		Size: 10.2 MB (10218017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801295d59b33e19109e93ada5f5bd22493781b3b4427766642f38297fd9a394f`  
		Last Modified: Fri, 29 Jul 2022 21:46:40 GMT  
		Size: 17.5 MB (17462132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281582a6a59d8bf62488abef853dd03ba854dcd8e11e36253bdacbbb59a16d7a`  
		Last Modified: Fri, 29 Jul 2022 21:46:36 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9124a342e40a4f75161fc22c685fb34f809d40655e6101d9916aa7dc23cc7831`  
		Last Modified: Fri, 29 Jul 2022 21:47:01 GMT  
		Size: 37.9 MB (37921681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eda0d8e6413bd60164de91e7ccaafb374de56761659d815d697fc383909cd2a`  
		Last Modified: Fri, 29 Jul 2022 21:46:54 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.22.4` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:a0b83997ae451a71613dc728fdf1dd9518707c62b01eb2d4754d48812f8f7000
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.7 MB (124686348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97bde2495b78fced58e8c1cba9862d4d0e9c08a803de66d5e938a829a26e184e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:24 GMT
ADD file:5972a7ce0f1d89d63e5ed48011838c998fa506cd34f8e5f0b0070039cd74c5b9 in / 
# Tue, 02 Aug 2022 00:40:25 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:24:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:24:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 22:58:27 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 22:58:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 02 Aug 2022 22:58:43 GMT
ENV TELEGRAF_VERSION=1.22.4
# Tue, 02 Aug 2022 22:58:48 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 02 Aug 2022 22:58:49 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 02 Aug 2022 22:58:50 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 02 Aug 2022 22:58:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 Aug 2022 22:58:51 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:114ba63dd73a866ac1bb59fe594dfd218f44ac9b4fa4b2c68499da5584fcfa9d`  
		Last Modified: Tue, 02 Aug 2022 00:45:33 GMT  
		Size: 53.7 MB (53683005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0b8a8acead4d7bf71c232054b2a0a8e08eb3e1e2cf46f9f3dba68723e88c85`  
		Last Modified: Tue, 02 Aug 2022 01:44:32 GMT  
		Size: 5.1 MB (5148901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ea641ee67989acdb6af3d8b9b984ecd751a2a83c3b7ce071542b31c9ac1304`  
		Last Modified: Tue, 02 Aug 2022 01:44:33 GMT  
		Size: 10.7 MB (10657494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b22bb61739a9b58a9acd5e791a783e60521e183266080deabfebd494ebb04a`  
		Last Modified: Tue, 02 Aug 2022 22:59:29 GMT  
		Size: 18.4 MB (18382753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7992c681678681934e95ece4d739305c6598ac402216ea7726cbdc2e2f758516`  
		Last Modified: Tue, 02 Aug 2022 22:59:26 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5787a3b346b420e74710d87245793734fd3277af3ec6274a2f4e8ad5f0183e9`  
		Last Modified: Tue, 02 Aug 2022 22:59:49 GMT  
		Size: 36.8 MB (36810994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be79842777b5861a646af4982b864132e2f8752e8bee0675d882ed12853fd202`  
		Last Modified: Tue, 02 Aug 2022 22:59:43 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.22.4-alpine`

```console
$ docker pull telegraf@sha256:bf27934d3967ab34011854e1951b00cd30218ff49d5e30512dada3a568782606
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.22.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:c9c0e1f082fc573fb815361cce09bdd05f4756ba427d445b3a3a9a6c060239fa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.5 MB (46542137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9d178f642164168fecf5d636292cca6a61d896c8723830cf3717c3f3fd992c9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 02:25:55 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 20 Jul 2022 02:25:58 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 20 Jul 2022 02:26:08 GMT
ENV TELEGRAF_VERSION=1.22.4
# Wed, 20 Jul 2022 02:26:15 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 20 Jul 2022 02:26:15 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 20 Jul 2022 02:26:15 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 20 Jul 2022 02:26:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 20 Jul 2022 02:26:15 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1d6c3bdc90884e20be4b8964afbc50fc83dac03969c542117bb4c4e59802fb`  
		Last Modified: Wed, 20 Jul 2022 02:26:48 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7afda0100e244bcaa7520aff1df3205abf84be1593c127ee83151d1395be22`  
		Last Modified: Wed, 20 Jul 2022 02:26:49 GMT  
		Size: 3.4 MB (3372891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1744c6d7f1d3b0cfc79904e1d04f119570f1aa76386244b2a87426468fd4d500`  
		Last Modified: Wed, 20 Jul 2022 02:27:11 GMT  
		Size: 40.4 MB (40354121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:702b42dd6a8e2c24a184819f51f5ba8fa12e92b225839733cc72571c871ba5a1`  
		Last Modified: Wed, 20 Jul 2022 02:27:05 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.23`

```console
$ docker pull telegraf@sha256:4309caa2d5f980ee1ef31a01f251b426ccb3e6a03be4070ceeddb745311305a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.23` - linux; amd64

```console
$ docker pull telegraf@sha256:371c9d2a91b7508cccce0fbd7583afdf1b6aa37a43c704a28f8f559fd54d7d30
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131476092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb9b6d06dcaba73e3a89dae5e0d6de8413e50044aa8f36d9066b813f506292a9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 02 Aug 2022 01:19:54 GMT
ADD file:d0f758e50c654c225f6c7f03e8a579efc9106437051573bdbae5e63b1c4b2c1f in / 
# Tue, 02 Aug 2022 01:19:54 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:46:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:47:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 03 Aug 2022 02:19:18 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 02:19:20 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 Aug 2022 02:19:38 GMT
ENV TELEGRAF_VERSION=1.23.3
# Wed, 03 Aug 2022 02:19:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 Aug 2022 02:19:42 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 Aug 2022 02:19:43 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 Aug 2022 02:19:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 Aug 2022 02:19:43 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:001c52e26ad57e3b25b439ee0052f6692e5c0f2d5d982a00a8819ace5e521452`  
		Last Modified: Tue, 02 Aug 2022 01:23:44 GMT  
		Size: 55.0 MB (54999331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d4b9b6e964657da49910b495173d6c4f0d9bc47b3b44273cf82fd32723d165`  
		Last Modified: Tue, 02 Aug 2022 02:18:26 GMT  
		Size: 5.2 MB (5156256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2068746827ec1b043b571e4788693eab7e9b2a95301176512791f8c317a2816a`  
		Last Modified: Tue, 02 Aug 2022 02:18:26 GMT  
		Size: 10.9 MB (10876485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fa4837c01bf0ec37537e86b40953e1be0c5a2f73ab15bb8d9267c641f2937c`  
		Last Modified: Wed, 03 Aug 2022 02:20:07 GMT  
		Size: 18.8 MB (18760336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78684b72b16c9b01fb02bc8c8f26552e94b5655a2a12226c010bc75c8dd0a514`  
		Last Modified: Wed, 03 Aug 2022 02:20:04 GMT  
		Size: 2.9 KB (2902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060eb4fe3af63f0b6600e68be9211b8c5c7aa278ba84949cf66df206d51d4c78`  
		Last Modified: Wed, 03 Aug 2022 02:20:46 GMT  
		Size: 41.7 MB (41680438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2bd2ae1d98c17167d30adcf69fc8ed80b5c2072dd2ec4feb8a07a45748341f4`  
		Last Modified: Wed, 03 Aug 2022 02:20:39 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:979a4110f2ba73ab38ab0c6992051d9d5fd73967451afdd5989d3e232d9f457a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121774975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f0b9edcbb93f865877c9f27012fba4f5828701ab9500a50bc807969c7d945c7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:16 GMT
ADD file:72ef8362158fcd45f10c6fa2dc3ea411e81f700ecb92faf37cb6dc1887756f9d in / 
# Tue, 12 Jul 2022 00:59:17 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 13:25:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 13:26:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Jul 2022 21:45:39 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2022 21:45:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 29 Jul 2022 21:46:03 GMT
ENV TELEGRAF_VERSION=1.23.3
# Fri, 29 Jul 2022 21:46:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 29 Jul 2022 21:46:09 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 29 Jul 2022 21:46:09 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 29 Jul 2022 21:46:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Jul 2022 21:46:09 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a8a55ed160b9a554de2e46b828d606a0829d8d9f19c79bc47eddac683aeb2b91`  
		Last Modified: Tue, 12 Jul 2022 01:11:51 GMT  
		Size: 50.2 MB (50194881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de0d7ddb0c03f1180487d49fda757592276a2a2eedc3f36d7bd625e1de85cc4`  
		Last Modified: Thu, 28 Jul 2022 13:52:28 GMT  
		Size: 4.9 MB (4924805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc57b4c2f87bc9e41a073ca20fcc00a5105e1147f67f5968e36f843fff2da78a`  
		Last Modified: Thu, 28 Jul 2022 13:52:29 GMT  
		Size: 10.2 MB (10218017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801295d59b33e19109e93ada5f5bd22493781b3b4427766642f38297fd9a394f`  
		Last Modified: Fri, 29 Jul 2022 21:46:40 GMT  
		Size: 17.5 MB (17462132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281582a6a59d8bf62488abef853dd03ba854dcd8e11e36253bdacbbb59a16d7a`  
		Last Modified: Fri, 29 Jul 2022 21:46:36 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0350eabc79817fb200a211759039bd114d6b57ab7d3031c623b8a959d8ee5b`  
		Last Modified: Fri, 29 Jul 2022 21:47:19 GMT  
		Size: 39.0 MB (38971909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240f2b7addc473af0a9c0a4e6f3934959f629b5beac6c342e0f7abe4da362232`  
		Last Modified: Fri, 29 Jul 2022 21:47:12 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:f2d2d85460ea628236d464d3736dd05818f6428be9630651c4c9df9f9b2e6130
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125748605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bd87442545488ce80f3efd47d91181dc00f9c2712d1beac9e5617fb5c0fe1b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:24 GMT
ADD file:5972a7ce0f1d89d63e5ed48011838c998fa506cd34f8e5f0b0070039cd74c5b9 in / 
# Tue, 02 Aug 2022 00:40:25 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:24:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:24:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 22:58:27 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 22:58:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 02 Aug 2022 22:58:57 GMT
ENV TELEGRAF_VERSION=1.23.3
# Tue, 02 Aug 2022 22:59:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 02 Aug 2022 22:59:01 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 02 Aug 2022 22:59:03 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 02 Aug 2022 22:59:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 Aug 2022 22:59:04 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:114ba63dd73a866ac1bb59fe594dfd218f44ac9b4fa4b2c68499da5584fcfa9d`  
		Last Modified: Tue, 02 Aug 2022 00:45:33 GMT  
		Size: 53.7 MB (53683005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0b8a8acead4d7bf71c232054b2a0a8e08eb3e1e2cf46f9f3dba68723e88c85`  
		Last Modified: Tue, 02 Aug 2022 01:44:32 GMT  
		Size: 5.1 MB (5148901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ea641ee67989acdb6af3d8b9b984ecd751a2a83c3b7ce071542b31c9ac1304`  
		Last Modified: Tue, 02 Aug 2022 01:44:33 GMT  
		Size: 10.7 MB (10657494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b22bb61739a9b58a9acd5e791a783e60521e183266080deabfebd494ebb04a`  
		Last Modified: Tue, 02 Aug 2022 22:59:29 GMT  
		Size: 18.4 MB (18382753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7992c681678681934e95ece4d739305c6598ac402216ea7726cbdc2e2f758516`  
		Last Modified: Tue, 02 Aug 2022 22:59:26 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2da7819eca7b7dc5f950f25343eed6dbd929ee5466ea17512549380d94272fe`  
		Last Modified: Tue, 02 Aug 2022 23:00:05 GMT  
		Size: 37.9 MB (37873252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e932c7189d58c551aeac0b76b5f836eedcd80604914b88528fac47f48ea317`  
		Last Modified: Tue, 02 Aug 2022 22:59:59 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.23-alpine`

```console
$ docker pull telegraf@sha256:c68155d27ef47740a4f1db5be56e4f5d3694897912a5ed7a12f6f56253fa7f40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.23-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:02bd3d2fa0ab0a7723591bb63b0f72bc822908d7aa94affd988578e195c9c89e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47704348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75df61c63ea56d73f573615a74aa8b036c7ba39d6bd87285b596eb105862ce4c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 02:25:55 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 20 Jul 2022 02:25:58 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 25 Jul 2022 19:26:00 GMT
ENV TELEGRAF_VERSION=1.23.3
# Mon, 25 Jul 2022 19:26:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 25 Jul 2022 19:26:06 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 25 Jul 2022 19:26:06 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 25 Jul 2022 19:26:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 25 Jul 2022 19:26:06 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1d6c3bdc90884e20be4b8964afbc50fc83dac03969c542117bb4c4e59802fb`  
		Last Modified: Wed, 20 Jul 2022 02:26:48 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7afda0100e244bcaa7520aff1df3205abf84be1593c127ee83151d1395be22`  
		Last Modified: Wed, 20 Jul 2022 02:26:49 GMT  
		Size: 3.4 MB (3372891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b37b8327c7da97731badaac61f32b1ebf831dcce280958d363f38a19afd2dd`  
		Last Modified: Mon, 25 Jul 2022 19:26:56 GMT  
		Size: 41.5 MB (41516332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793a8b0315f1b7be062391b8807dbed99fd4ed5810d0f34323b8c00a4c42466a`  
		Last Modified: Mon, 25 Jul 2022 19:26:49 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.23.3`

```console
$ docker pull telegraf@sha256:4309caa2d5f980ee1ef31a01f251b426ccb3e6a03be4070ceeddb745311305a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.23.3` - linux; amd64

```console
$ docker pull telegraf@sha256:371c9d2a91b7508cccce0fbd7583afdf1b6aa37a43c704a28f8f559fd54d7d30
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131476092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb9b6d06dcaba73e3a89dae5e0d6de8413e50044aa8f36d9066b813f506292a9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 02 Aug 2022 01:19:54 GMT
ADD file:d0f758e50c654c225f6c7f03e8a579efc9106437051573bdbae5e63b1c4b2c1f in / 
# Tue, 02 Aug 2022 01:19:54 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:46:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:47:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 03 Aug 2022 02:19:18 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 02:19:20 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 Aug 2022 02:19:38 GMT
ENV TELEGRAF_VERSION=1.23.3
# Wed, 03 Aug 2022 02:19:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 Aug 2022 02:19:42 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 Aug 2022 02:19:43 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 Aug 2022 02:19:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 Aug 2022 02:19:43 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:001c52e26ad57e3b25b439ee0052f6692e5c0f2d5d982a00a8819ace5e521452`  
		Last Modified: Tue, 02 Aug 2022 01:23:44 GMT  
		Size: 55.0 MB (54999331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d4b9b6e964657da49910b495173d6c4f0d9bc47b3b44273cf82fd32723d165`  
		Last Modified: Tue, 02 Aug 2022 02:18:26 GMT  
		Size: 5.2 MB (5156256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2068746827ec1b043b571e4788693eab7e9b2a95301176512791f8c317a2816a`  
		Last Modified: Tue, 02 Aug 2022 02:18:26 GMT  
		Size: 10.9 MB (10876485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fa4837c01bf0ec37537e86b40953e1be0c5a2f73ab15bb8d9267c641f2937c`  
		Last Modified: Wed, 03 Aug 2022 02:20:07 GMT  
		Size: 18.8 MB (18760336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78684b72b16c9b01fb02bc8c8f26552e94b5655a2a12226c010bc75c8dd0a514`  
		Last Modified: Wed, 03 Aug 2022 02:20:04 GMT  
		Size: 2.9 KB (2902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060eb4fe3af63f0b6600e68be9211b8c5c7aa278ba84949cf66df206d51d4c78`  
		Last Modified: Wed, 03 Aug 2022 02:20:46 GMT  
		Size: 41.7 MB (41680438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2bd2ae1d98c17167d30adcf69fc8ed80b5c2072dd2ec4feb8a07a45748341f4`  
		Last Modified: Wed, 03 Aug 2022 02:20:39 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23.3` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:979a4110f2ba73ab38ab0c6992051d9d5fd73967451afdd5989d3e232d9f457a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121774975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f0b9edcbb93f865877c9f27012fba4f5828701ab9500a50bc807969c7d945c7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:16 GMT
ADD file:72ef8362158fcd45f10c6fa2dc3ea411e81f700ecb92faf37cb6dc1887756f9d in / 
# Tue, 12 Jul 2022 00:59:17 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 13:25:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 13:26:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Jul 2022 21:45:39 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2022 21:45:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 29 Jul 2022 21:46:03 GMT
ENV TELEGRAF_VERSION=1.23.3
# Fri, 29 Jul 2022 21:46:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 29 Jul 2022 21:46:09 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 29 Jul 2022 21:46:09 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 29 Jul 2022 21:46:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Jul 2022 21:46:09 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a8a55ed160b9a554de2e46b828d606a0829d8d9f19c79bc47eddac683aeb2b91`  
		Last Modified: Tue, 12 Jul 2022 01:11:51 GMT  
		Size: 50.2 MB (50194881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de0d7ddb0c03f1180487d49fda757592276a2a2eedc3f36d7bd625e1de85cc4`  
		Last Modified: Thu, 28 Jul 2022 13:52:28 GMT  
		Size: 4.9 MB (4924805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc57b4c2f87bc9e41a073ca20fcc00a5105e1147f67f5968e36f843fff2da78a`  
		Last Modified: Thu, 28 Jul 2022 13:52:29 GMT  
		Size: 10.2 MB (10218017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801295d59b33e19109e93ada5f5bd22493781b3b4427766642f38297fd9a394f`  
		Last Modified: Fri, 29 Jul 2022 21:46:40 GMT  
		Size: 17.5 MB (17462132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281582a6a59d8bf62488abef853dd03ba854dcd8e11e36253bdacbbb59a16d7a`  
		Last Modified: Fri, 29 Jul 2022 21:46:36 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0350eabc79817fb200a211759039bd114d6b57ab7d3031c623b8a959d8ee5b`  
		Last Modified: Fri, 29 Jul 2022 21:47:19 GMT  
		Size: 39.0 MB (38971909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240f2b7addc473af0a9c0a4e6f3934959f629b5beac6c342e0f7abe4da362232`  
		Last Modified: Fri, 29 Jul 2022 21:47:12 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23.3` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:f2d2d85460ea628236d464d3736dd05818f6428be9630651c4c9df9f9b2e6130
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125748605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bd87442545488ce80f3efd47d91181dc00f9c2712d1beac9e5617fb5c0fe1b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:24 GMT
ADD file:5972a7ce0f1d89d63e5ed48011838c998fa506cd34f8e5f0b0070039cd74c5b9 in / 
# Tue, 02 Aug 2022 00:40:25 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:24:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:24:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 22:58:27 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 22:58:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 02 Aug 2022 22:58:57 GMT
ENV TELEGRAF_VERSION=1.23.3
# Tue, 02 Aug 2022 22:59:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 02 Aug 2022 22:59:01 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 02 Aug 2022 22:59:03 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 02 Aug 2022 22:59:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 Aug 2022 22:59:04 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:114ba63dd73a866ac1bb59fe594dfd218f44ac9b4fa4b2c68499da5584fcfa9d`  
		Last Modified: Tue, 02 Aug 2022 00:45:33 GMT  
		Size: 53.7 MB (53683005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0b8a8acead4d7bf71c232054b2a0a8e08eb3e1e2cf46f9f3dba68723e88c85`  
		Last Modified: Tue, 02 Aug 2022 01:44:32 GMT  
		Size: 5.1 MB (5148901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ea641ee67989acdb6af3d8b9b984ecd751a2a83c3b7ce071542b31c9ac1304`  
		Last Modified: Tue, 02 Aug 2022 01:44:33 GMT  
		Size: 10.7 MB (10657494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b22bb61739a9b58a9acd5e791a783e60521e183266080deabfebd494ebb04a`  
		Last Modified: Tue, 02 Aug 2022 22:59:29 GMT  
		Size: 18.4 MB (18382753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7992c681678681934e95ece4d739305c6598ac402216ea7726cbdc2e2f758516`  
		Last Modified: Tue, 02 Aug 2022 22:59:26 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2da7819eca7b7dc5f950f25343eed6dbd929ee5466ea17512549380d94272fe`  
		Last Modified: Tue, 02 Aug 2022 23:00:05 GMT  
		Size: 37.9 MB (37873252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e932c7189d58c551aeac0b76b5f836eedcd80604914b88528fac47f48ea317`  
		Last Modified: Tue, 02 Aug 2022 22:59:59 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.23.3-alpine`

```console
$ docker pull telegraf@sha256:c68155d27ef47740a4f1db5be56e4f5d3694897912a5ed7a12f6f56253fa7f40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.23.3-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:02bd3d2fa0ab0a7723591bb63b0f72bc822908d7aa94affd988578e195c9c89e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47704348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75df61c63ea56d73f573615a74aa8b036c7ba39d6bd87285b596eb105862ce4c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 02:25:55 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 20 Jul 2022 02:25:58 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 25 Jul 2022 19:26:00 GMT
ENV TELEGRAF_VERSION=1.23.3
# Mon, 25 Jul 2022 19:26:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 25 Jul 2022 19:26:06 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 25 Jul 2022 19:26:06 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 25 Jul 2022 19:26:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 25 Jul 2022 19:26:06 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1d6c3bdc90884e20be4b8964afbc50fc83dac03969c542117bb4c4e59802fb`  
		Last Modified: Wed, 20 Jul 2022 02:26:48 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7afda0100e244bcaa7520aff1df3205abf84be1593c127ee83151d1395be22`  
		Last Modified: Wed, 20 Jul 2022 02:26:49 GMT  
		Size: 3.4 MB (3372891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b37b8327c7da97731badaac61f32b1ebf831dcce280958d363f38a19afd2dd`  
		Last Modified: Mon, 25 Jul 2022 19:26:56 GMT  
		Size: 41.5 MB (41516332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793a8b0315f1b7be062391b8807dbed99fd4ed5810d0f34323b8c00a4c42466a`  
		Last Modified: Mon, 25 Jul 2022 19:26:49 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:c68155d27ef47740a4f1db5be56e4f5d3694897912a5ed7a12f6f56253fa7f40
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:02bd3d2fa0ab0a7723591bb63b0f72bc822908d7aa94affd988578e195c9c89e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47704348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75df61c63ea56d73f573615a74aa8b036c7ba39d6bd87285b596eb105862ce4c`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:11 GMT
ADD file:c679662d1fba5d188d8f31ab4ebeb7099221926df7630a6917aa461fc33d7ea6 in / 
# Tue, 19 Jul 2022 22:20:11 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 02:25:55 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 20 Jul 2022 02:25:58 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 25 Jul 2022 19:26:00 GMT
ENV TELEGRAF_VERSION=1.23.3
# Mon, 25 Jul 2022 19:26:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 25 Jul 2022 19:26:06 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 25 Jul 2022 19:26:06 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 25 Jul 2022 19:26:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 25 Jul 2022 19:26:06 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ab6db1bc80d0a6df92d04c3fad44b9443642fbc85878023bc8c011763fe44524`  
		Last Modified: Tue, 19 Jul 2022 22:20:46 GMT  
		Size: 2.8 MB (2814645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1d6c3bdc90884e20be4b8964afbc50fc83dac03969c542117bb4c4e59802fb`  
		Last Modified: Wed, 20 Jul 2022 02:26:48 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7afda0100e244bcaa7520aff1df3205abf84be1593c127ee83151d1395be22`  
		Last Modified: Wed, 20 Jul 2022 02:26:49 GMT  
		Size: 3.4 MB (3372891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b37b8327c7da97731badaac61f32b1ebf831dcce280958d363f38a19afd2dd`  
		Last Modified: Mon, 25 Jul 2022 19:26:56 GMT  
		Size: 41.5 MB (41516332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793a8b0315f1b7be062391b8807dbed99fd4ed5810d0f34323b8c00a4c42466a`  
		Last Modified: Mon, 25 Jul 2022 19:26:49 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:4309caa2d5f980ee1ef31a01f251b426ccb3e6a03be4070ceeddb745311305a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:371c9d2a91b7508cccce0fbd7583afdf1b6aa37a43c704a28f8f559fd54d7d30
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131476092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb9b6d06dcaba73e3a89dae5e0d6de8413e50044aa8f36d9066b813f506292a9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 02 Aug 2022 01:19:54 GMT
ADD file:d0f758e50c654c225f6c7f03e8a579efc9106437051573bdbae5e63b1c4b2c1f in / 
# Tue, 02 Aug 2022 01:19:54 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:46:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:47:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 03 Aug 2022 02:19:18 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 02:19:20 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 Aug 2022 02:19:38 GMT
ENV TELEGRAF_VERSION=1.23.3
# Wed, 03 Aug 2022 02:19:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 Aug 2022 02:19:42 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 Aug 2022 02:19:43 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 Aug 2022 02:19:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 Aug 2022 02:19:43 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:001c52e26ad57e3b25b439ee0052f6692e5c0f2d5d982a00a8819ace5e521452`  
		Last Modified: Tue, 02 Aug 2022 01:23:44 GMT  
		Size: 55.0 MB (54999331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d4b9b6e964657da49910b495173d6c4f0d9bc47b3b44273cf82fd32723d165`  
		Last Modified: Tue, 02 Aug 2022 02:18:26 GMT  
		Size: 5.2 MB (5156256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2068746827ec1b043b571e4788693eab7e9b2a95301176512791f8c317a2816a`  
		Last Modified: Tue, 02 Aug 2022 02:18:26 GMT  
		Size: 10.9 MB (10876485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0fa4837c01bf0ec37537e86b40953e1be0c5a2f73ab15bb8d9267c641f2937c`  
		Last Modified: Wed, 03 Aug 2022 02:20:07 GMT  
		Size: 18.8 MB (18760336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78684b72b16c9b01fb02bc8c8f26552e94b5655a2a12226c010bc75c8dd0a514`  
		Last Modified: Wed, 03 Aug 2022 02:20:04 GMT  
		Size: 2.9 KB (2902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060eb4fe3af63f0b6600e68be9211b8c5c7aa278ba84949cf66df206d51d4c78`  
		Last Modified: Wed, 03 Aug 2022 02:20:46 GMT  
		Size: 41.7 MB (41680438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2bd2ae1d98c17167d30adcf69fc8ed80b5c2072dd2ec4feb8a07a45748341f4`  
		Last Modified: Wed, 03 Aug 2022 02:20:39 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:979a4110f2ba73ab38ab0c6992051d9d5fd73967451afdd5989d3e232d9f457a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121774975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f0b9edcbb93f865877c9f27012fba4f5828701ab9500a50bc807969c7d945c7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:16 GMT
ADD file:72ef8362158fcd45f10c6fa2dc3ea411e81f700ecb92faf37cb6dc1887756f9d in / 
# Tue, 12 Jul 2022 00:59:17 GMT
CMD ["bash"]
# Thu, 28 Jul 2022 13:25:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 28 Jul 2022 13:26:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Jul 2022 21:45:39 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 29 Jul 2022 21:45:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 29 Jul 2022 21:46:03 GMT
ENV TELEGRAF_VERSION=1.23.3
# Fri, 29 Jul 2022 21:46:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 29 Jul 2022 21:46:09 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 29 Jul 2022 21:46:09 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 29 Jul 2022 21:46:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 29 Jul 2022 21:46:09 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a8a55ed160b9a554de2e46b828d606a0829d8d9f19c79bc47eddac683aeb2b91`  
		Last Modified: Tue, 12 Jul 2022 01:11:51 GMT  
		Size: 50.2 MB (50194881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7de0d7ddb0c03f1180487d49fda757592276a2a2eedc3f36d7bd625e1de85cc4`  
		Last Modified: Thu, 28 Jul 2022 13:52:28 GMT  
		Size: 4.9 MB (4924805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc57b4c2f87bc9e41a073ca20fcc00a5105e1147f67f5968e36f843fff2da78a`  
		Last Modified: Thu, 28 Jul 2022 13:52:29 GMT  
		Size: 10.2 MB (10218017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801295d59b33e19109e93ada5f5bd22493781b3b4427766642f38297fd9a394f`  
		Last Modified: Fri, 29 Jul 2022 21:46:40 GMT  
		Size: 17.5 MB (17462132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281582a6a59d8bf62488abef853dd03ba854dcd8e11e36253bdacbbb59a16d7a`  
		Last Modified: Fri, 29 Jul 2022 21:46:36 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0350eabc79817fb200a211759039bd114d6b57ab7d3031c623b8a959d8ee5b`  
		Last Modified: Fri, 29 Jul 2022 21:47:19 GMT  
		Size: 39.0 MB (38971909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240f2b7addc473af0a9c0a4e6f3934959f629b5beac6c342e0f7abe4da362232`  
		Last Modified: Fri, 29 Jul 2022 21:47:12 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:f2d2d85460ea628236d464d3736dd05818f6428be9630651c4c9df9f9b2e6130
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125748605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bd87442545488ce80f3efd47d91181dc00f9c2712d1beac9e5617fb5c0fe1b1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:24 GMT
ADD file:5972a7ce0f1d89d63e5ed48011838c998fa506cd34f8e5f0b0070039cd74c5b9 in / 
# Tue, 02 Aug 2022 00:40:25 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:24:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:24:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 22:58:27 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 22:58:29 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 02 Aug 2022 22:58:57 GMT
ENV TELEGRAF_VERSION=1.23.3
# Tue, 02 Aug 2022 22:59:01 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 02 Aug 2022 22:59:01 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 02 Aug 2022 22:59:03 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 02 Aug 2022 22:59:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 02 Aug 2022 22:59:04 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:114ba63dd73a866ac1bb59fe594dfd218f44ac9b4fa4b2c68499da5584fcfa9d`  
		Last Modified: Tue, 02 Aug 2022 00:45:33 GMT  
		Size: 53.7 MB (53683005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0b8a8acead4d7bf71c232054b2a0a8e08eb3e1e2cf46f9f3dba68723e88c85`  
		Last Modified: Tue, 02 Aug 2022 01:44:32 GMT  
		Size: 5.1 MB (5148901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ea641ee67989acdb6af3d8b9b984ecd751a2a83c3b7ce071542b31c9ac1304`  
		Last Modified: Tue, 02 Aug 2022 01:44:33 GMT  
		Size: 10.7 MB (10657494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b22bb61739a9b58a9acd5e791a783e60521e183266080deabfebd494ebb04a`  
		Last Modified: Tue, 02 Aug 2022 22:59:29 GMT  
		Size: 18.4 MB (18382753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7992c681678681934e95ece4d739305c6598ac402216ea7726cbdc2e2f758516`  
		Last Modified: Tue, 02 Aug 2022 22:59:26 GMT  
		Size: 2.9 KB (2859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2da7819eca7b7dc5f950f25343eed6dbd929ee5466ea17512549380d94272fe`  
		Last Modified: Tue, 02 Aug 2022 23:00:05 GMT  
		Size: 37.9 MB (37873252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e932c7189d58c551aeac0b76b5f836eedcd80604914b88528fac47f48ea317`  
		Last Modified: Tue, 02 Aug 2022 22:59:59 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
