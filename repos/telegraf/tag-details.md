<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `telegraf`

-	[`telegraf:1.22`](#telegraf122)
-	[`telegraf:1.22-alpine`](#telegraf122-alpine)
-	[`telegraf:1.22.4`](#telegraf1224)
-	[`telegraf:1.22.4-alpine`](#telegraf1224-alpine)
-	[`telegraf:1.23`](#telegraf123)
-	[`telegraf:1.23-alpine`](#telegraf123-alpine)
-	[`telegraf:1.23.4`](#telegraf1234)
-	[`telegraf:1.23.4-alpine`](#telegraf1234-alpine)
-	[`telegraf:1.24`](#telegraf124)
-	[`telegraf:1.24-alpine`](#telegraf124-alpine)
-	[`telegraf:1.24.0`](#telegraf1240)
-	[`telegraf:1.24.0-alpine`](#telegraf1240-alpine)
-	[`telegraf:alpine`](#telegrafalpine)
-	[`telegraf:latest`](#telegraflatest)

## `telegraf:1.22`

```console
$ docker pull telegraf@sha256:ed9f1b0b2f25059edcb247aa54d312d8181e863cbfdcf0a4ea5efaca4d97e03c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.22` - linux; amd64

```console
$ docker pull telegraf@sha256:b2f057d002a2ec7d424a8270fdde6392ef903e31ac3a9f135366af1551f615e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.3 MB (130308935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88d6a91dae8784279a3582b4bb093b8cda77ce9503b3c7acabcc9e27b36f5a20`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:48:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 20:18:39 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 20:18:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 23 Aug 2022 20:18:51 GMT
ENV TELEGRAF_VERSION=1.22.4
# Tue, 23 Aug 2022 20:18:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 23 Aug 2022 20:18:55 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 23 Aug 2022 20:18:55 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 23 Aug 2022 20:18:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 Aug 2022 20:18:55 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e94d13e55e7a4ef17ff21376f57fb95c7e1706931f8704aa99260968d81f6e4`  
		Last Modified: Tue, 23 Aug 2022 00:55:37 GMT  
		Size: 5.2 MB (5163019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9c7528c685216129e8e67bf362a7702e7b1daa585ab85546a41508830657d6`  
		Last Modified: Tue, 23 Aug 2022 00:55:38 GMT  
		Size: 10.9 MB (10876472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bf78e724b533506c47d613e8c51e7756df404678ac937fb012ecd677818fe8`  
		Last Modified: Tue, 23 Aug 2022 20:19:29 GMT  
		Size: 18.8 MB (18759919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320b93d95aa1cf3f1430c41fd73db6dbce1a9555be411bdc7b8beb2ccd712412`  
		Last Modified: Tue, 23 Aug 2022 20:19:25 GMT  
		Size: 2.9 KB (2903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa87c7041566d98f64d2616aa1271303d2f239c22a9bcf2c60b0af6d36e17c7`  
		Last Modified: Tue, 23 Aug 2022 20:19:50 GMT  
		Size: 40.5 MB (40498723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd77ace60c5cf82cf5760fad8806309c43892348566deb9f79843489840ff261`  
		Last Modified: Tue, 23 Aug 2022 20:19:43 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.22` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:c5032ca887c62a6c39660f064d007987020f3dbabdc0f6f8db42a0c687ea0338
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.7 MB (120740832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82a6bd0f2aa522d544fb76f1d38ae1f53bd82c1b15a81daf66d23f727bdfbd19`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:43 GMT
ADD file:21190c24a038c3c9de64b88797bf00e4c4319bd598c7c465cab2ca88d0502416 in / 
# Tue, 23 Aug 2022 01:42:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:59:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:00:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 24 Aug 2022 17:14:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 17:14:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 24 Aug 2022 17:14:24 GMT
ENV TELEGRAF_VERSION=1.22.4
# Wed, 24 Aug 2022 17:14:29 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 24 Aug 2022 17:14:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 24 Aug 2022 17:14:30 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 24 Aug 2022 17:14:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Aug 2022 17:14:30 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:c715a126a4d5182c28d2d7b1c81de847bfbbacf6851819fef3eb28e3feb7db0e`  
		Last Modified: Tue, 23 Aug 2022 01:49:30 GMT  
		Size: 50.2 MB (50204931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cecc62e275236714359bda7d1f9c8412e8fa8539f3ef682eebd9c77986c927d`  
		Last Modified: Tue, 23 Aug 2022 13:11:58 GMT  
		Size: 4.9 MB (4930827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818eb872fe75602d611beeac0db63da0a4d8a67aee8b909d5114814f76446a5e`  
		Last Modified: Tue, 23 Aug 2022 13:11:59 GMT  
		Size: 10.2 MB (10217900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28127e82dbad78eb691a0fb5e5374c2f1c2c7d4f9826ef923493608b5b98fb3c`  
		Last Modified: Wed, 24 Aug 2022 17:15:12 GMT  
		Size: 17.5 MB (17462272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a8e2427f6ebb3290b16701a3683670b1b092f3fb657747570316664b57f8e0`  
		Last Modified: Wed, 24 Aug 2022 17:15:08 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c544fef23fe2e946cb72d0a32732e5bfa8f5dfefaf81df81418f85d02e0414e9`  
		Last Modified: Wed, 24 Aug 2022 17:15:33 GMT  
		Size: 37.9 MB (37921671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070b8eae645d69f668b884fcb3600d73cd55841693ae96de8137e7189911b6a3`  
		Last Modified: Wed, 24 Aug 2022 17:15:26 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.22` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:8da29e2f75ee2ad2bcf1ed3dd31db02e4adea72bad625ded0033ca471fd67ead
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.5 MB (124489339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51dee7020c2d6bd5822b709f2fc9ac7be8ec20701f327f16415db9c1a0e0ce76`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:16 GMT
ADD file:ce6014a27d18915dc6d46c5c1f0f894f0027d1e41fbebb1599c16371b7bab2f1 in / 
# Tue, 23 Aug 2022 01:52:18 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:27:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 21:31:59 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 21:32:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 23 Aug 2022 21:32:15 GMT
ENV TELEGRAF_VERSION=1.22.4
# Tue, 23 Aug 2022 21:32:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 23 Aug 2022 21:32:20 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 23 Aug 2022 21:32:22 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 23 Aug 2022 21:32:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 Aug 2022 21:32:23 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:cd84405c8b9e7a8c3d580c2148d25120dd697ea61e1cb55a62f33e67988b7043`  
		Last Modified: Tue, 23 Aug 2022 01:57:29 GMT  
		Size: 53.7 MB (53690830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d98e120b809269e56de468d2b91569789c521011e4d9b1806e43fd04462de2`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 4.9 MB (4944180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb6be5911b40ca548e48c10b09cb2312f1698b4c84f09711c69389a94b1a8be`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 10.7 MB (10657442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab23840b45319a569927bb1e754dbbc4a1cd2644adaf7e32337156a0d803b491`  
		Last Modified: Tue, 23 Aug 2022 21:33:03 GMT  
		Size: 18.4 MB (18382761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8209f5a5eb7e11a25b57321f7e44a027d4c987c6abce3e24edf37b2184eb729`  
		Last Modified: Tue, 23 Aug 2022 21:33:00 GMT  
		Size: 2.9 KB (2858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a743f37002acb5f7af5785ca27661d5c24c936e8fe8bdef83ff0b459102cb48`  
		Last Modified: Tue, 23 Aug 2022 21:33:22 GMT  
		Size: 36.8 MB (36810923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173f39e7e262fad1e63c0cdfbb12127d90b3a71b4ef6647cc4c85a0b9cfa97ae`  
		Last Modified: Tue, 23 Aug 2022 21:33:17 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.22-alpine`

```console
$ docker pull telegraf@sha256:b1f729bad50e7043a30819550a6acc986dd98792f3184c8ddbb1e57b997b068c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.22-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:aa71936e9dcb7663d5416e09cbd2800d962cc5fcefb4ea023a45ece259fcc296
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.6 MB (46566277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69136d7106a90d17d873c40a2d210853da250899ace7ac834445d0e16d906fc0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:22:56 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 10 Aug 2022 01:22:58 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 10 Aug 2022 01:23:11 GMT
ENV TELEGRAF_VERSION=1.22.4
# Wed, 10 Aug 2022 01:23:17 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 10 Aug 2022 01:23:18 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 10 Aug 2022 01:23:18 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 10 Aug 2022 01:23:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Aug 2022 01:23:18 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b6e02c851cec1d59f28ff9497d3672a3b33ce39a9edb228b5744eb93372150`  
		Last Modified: Wed, 10 Aug 2022 01:23:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef163f69f1d36aa05f1f04751bf3169514539aa167c9094972f9987642270aab`  
		Last Modified: Wed, 10 Aug 2022 01:23:53 GMT  
		Size: 3.4 MB (3387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de74378a7b15880aa43d22249819805615dad98fa40a3e3673512b50c5138fd9`  
		Last Modified: Wed, 10 Aug 2022 01:24:17 GMT  
		Size: 40.4 MB (40354362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9637a38ca8f8fab4ecefe6f3913503012d2da45c1f9ea561c0d2d6dac0a44478`  
		Last Modified: Wed, 10 Aug 2022 01:24:10 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.22.4`

```console
$ docker pull telegraf@sha256:ed9f1b0b2f25059edcb247aa54d312d8181e863cbfdcf0a4ea5efaca4d97e03c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.22.4` - linux; amd64

```console
$ docker pull telegraf@sha256:b2f057d002a2ec7d424a8270fdde6392ef903e31ac3a9f135366af1551f615e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.3 MB (130308935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88d6a91dae8784279a3582b4bb093b8cda77ce9503b3c7acabcc9e27b36f5a20`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:48:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 20:18:39 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 20:18:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 23 Aug 2022 20:18:51 GMT
ENV TELEGRAF_VERSION=1.22.4
# Tue, 23 Aug 2022 20:18:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 23 Aug 2022 20:18:55 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 23 Aug 2022 20:18:55 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 23 Aug 2022 20:18:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 Aug 2022 20:18:55 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e94d13e55e7a4ef17ff21376f57fb95c7e1706931f8704aa99260968d81f6e4`  
		Last Modified: Tue, 23 Aug 2022 00:55:37 GMT  
		Size: 5.2 MB (5163019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9c7528c685216129e8e67bf362a7702e7b1daa585ab85546a41508830657d6`  
		Last Modified: Tue, 23 Aug 2022 00:55:38 GMT  
		Size: 10.9 MB (10876472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bf78e724b533506c47d613e8c51e7756df404678ac937fb012ecd677818fe8`  
		Last Modified: Tue, 23 Aug 2022 20:19:29 GMT  
		Size: 18.8 MB (18759919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320b93d95aa1cf3f1430c41fd73db6dbce1a9555be411bdc7b8beb2ccd712412`  
		Last Modified: Tue, 23 Aug 2022 20:19:25 GMT  
		Size: 2.9 KB (2903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa87c7041566d98f64d2616aa1271303d2f239c22a9bcf2c60b0af6d36e17c7`  
		Last Modified: Tue, 23 Aug 2022 20:19:50 GMT  
		Size: 40.5 MB (40498723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd77ace60c5cf82cf5760fad8806309c43892348566deb9f79843489840ff261`  
		Last Modified: Tue, 23 Aug 2022 20:19:43 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.22.4` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:c5032ca887c62a6c39660f064d007987020f3dbabdc0f6f8db42a0c687ea0338
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.7 MB (120740832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82a6bd0f2aa522d544fb76f1d38ae1f53bd82c1b15a81daf66d23f727bdfbd19`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:43 GMT
ADD file:21190c24a038c3c9de64b88797bf00e4c4319bd598c7c465cab2ca88d0502416 in / 
# Tue, 23 Aug 2022 01:42:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:59:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:00:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 24 Aug 2022 17:14:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 17:14:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 24 Aug 2022 17:14:24 GMT
ENV TELEGRAF_VERSION=1.22.4
# Wed, 24 Aug 2022 17:14:29 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 24 Aug 2022 17:14:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 24 Aug 2022 17:14:30 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 24 Aug 2022 17:14:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Aug 2022 17:14:30 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:c715a126a4d5182c28d2d7b1c81de847bfbbacf6851819fef3eb28e3feb7db0e`  
		Last Modified: Tue, 23 Aug 2022 01:49:30 GMT  
		Size: 50.2 MB (50204931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cecc62e275236714359bda7d1f9c8412e8fa8539f3ef682eebd9c77986c927d`  
		Last Modified: Tue, 23 Aug 2022 13:11:58 GMT  
		Size: 4.9 MB (4930827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818eb872fe75602d611beeac0db63da0a4d8a67aee8b909d5114814f76446a5e`  
		Last Modified: Tue, 23 Aug 2022 13:11:59 GMT  
		Size: 10.2 MB (10217900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28127e82dbad78eb691a0fb5e5374c2f1c2c7d4f9826ef923493608b5b98fb3c`  
		Last Modified: Wed, 24 Aug 2022 17:15:12 GMT  
		Size: 17.5 MB (17462272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a8e2427f6ebb3290b16701a3683670b1b092f3fb657747570316664b57f8e0`  
		Last Modified: Wed, 24 Aug 2022 17:15:08 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c544fef23fe2e946cb72d0a32732e5bfa8f5dfefaf81df81418f85d02e0414e9`  
		Last Modified: Wed, 24 Aug 2022 17:15:33 GMT  
		Size: 37.9 MB (37921671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:070b8eae645d69f668b884fcb3600d73cd55841693ae96de8137e7189911b6a3`  
		Last Modified: Wed, 24 Aug 2022 17:15:26 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.22.4` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:8da29e2f75ee2ad2bcf1ed3dd31db02e4adea72bad625ded0033ca471fd67ead
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.5 MB (124489339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51dee7020c2d6bd5822b709f2fc9ac7be8ec20701f327f16415db9c1a0e0ce76`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:16 GMT
ADD file:ce6014a27d18915dc6d46c5c1f0f894f0027d1e41fbebb1599c16371b7bab2f1 in / 
# Tue, 23 Aug 2022 01:52:18 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:27:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 21:31:59 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 21:32:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 23 Aug 2022 21:32:15 GMT
ENV TELEGRAF_VERSION=1.22.4
# Tue, 23 Aug 2022 21:32:20 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 23 Aug 2022 21:32:20 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 23 Aug 2022 21:32:22 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 23 Aug 2022 21:32:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 Aug 2022 21:32:23 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:cd84405c8b9e7a8c3d580c2148d25120dd697ea61e1cb55a62f33e67988b7043`  
		Last Modified: Tue, 23 Aug 2022 01:57:29 GMT  
		Size: 53.7 MB (53690830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d98e120b809269e56de468d2b91569789c521011e4d9b1806e43fd04462de2`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 4.9 MB (4944180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb6be5911b40ca548e48c10b09cb2312f1698b4c84f09711c69389a94b1a8be`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 10.7 MB (10657442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab23840b45319a569927bb1e754dbbc4a1cd2644adaf7e32337156a0d803b491`  
		Last Modified: Tue, 23 Aug 2022 21:33:03 GMT  
		Size: 18.4 MB (18382761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8209f5a5eb7e11a25b57321f7e44a027d4c987c6abce3e24edf37b2184eb729`  
		Last Modified: Tue, 23 Aug 2022 21:33:00 GMT  
		Size: 2.9 KB (2858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a743f37002acb5f7af5785ca27661d5c24c936e8fe8bdef83ff0b459102cb48`  
		Last Modified: Tue, 23 Aug 2022 21:33:22 GMT  
		Size: 36.8 MB (36810923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173f39e7e262fad1e63c0cdfbb12127d90b3a71b4ef6647cc4c85a0b9cfa97ae`  
		Last Modified: Tue, 23 Aug 2022 21:33:17 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.22.4-alpine`

```console
$ docker pull telegraf@sha256:b1f729bad50e7043a30819550a6acc986dd98792f3184c8ddbb1e57b997b068c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.22.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:aa71936e9dcb7663d5416e09cbd2800d962cc5fcefb4ea023a45ece259fcc296
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.6 MB (46566277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69136d7106a90d17d873c40a2d210853da250899ace7ac834445d0e16d906fc0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:22:56 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 10 Aug 2022 01:22:58 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 10 Aug 2022 01:23:11 GMT
ENV TELEGRAF_VERSION=1.22.4
# Wed, 10 Aug 2022 01:23:17 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 10 Aug 2022 01:23:18 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 10 Aug 2022 01:23:18 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 10 Aug 2022 01:23:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 10 Aug 2022 01:23:18 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b6e02c851cec1d59f28ff9497d3672a3b33ce39a9edb228b5744eb93372150`  
		Last Modified: Wed, 10 Aug 2022 01:23:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef163f69f1d36aa05f1f04751bf3169514539aa167c9094972f9987642270aab`  
		Last Modified: Wed, 10 Aug 2022 01:23:53 GMT  
		Size: 3.4 MB (3387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de74378a7b15880aa43d22249819805615dad98fa40a3e3673512b50c5138fd9`  
		Last Modified: Wed, 10 Aug 2022 01:24:17 GMT  
		Size: 40.4 MB (40354362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9637a38ca8f8fab4ecefe6f3913503012d2da45c1f9ea561c0d2d6dac0a44478`  
		Last Modified: Wed, 10 Aug 2022 01:24:10 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.23`

```console
$ docker pull telegraf@sha256:b2afad2ff2bb5b155d3ecc9f7037c51d9f505f535d1bc2569d625725ee3f8b2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.23` - linux; amd64

```console
$ docker pull telegraf@sha256:6579540446d8b48a68ee70a5d00aec0180a394b390f5c274192c125498befe80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131659359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7b77eb6d0523c0d58a999fb389e9023a81544aa60e91cd318e6d8d8d48240d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:48:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 20:18:39 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 20:18:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 23 Aug 2022 20:18:59 GMT
ENV TELEGRAF_VERSION=1.23.4
# Tue, 23 Aug 2022 20:19:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 23 Aug 2022 20:19:03 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 23 Aug 2022 20:19:04 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 23 Aug 2022 20:19:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 Aug 2022 20:19:04 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e94d13e55e7a4ef17ff21376f57fb95c7e1706931f8704aa99260968d81f6e4`  
		Last Modified: Tue, 23 Aug 2022 00:55:37 GMT  
		Size: 5.2 MB (5163019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9c7528c685216129e8e67bf362a7702e7b1daa585ab85546a41508830657d6`  
		Last Modified: Tue, 23 Aug 2022 00:55:38 GMT  
		Size: 10.9 MB (10876472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bf78e724b533506c47d613e8c51e7756df404678ac937fb012ecd677818fe8`  
		Last Modified: Tue, 23 Aug 2022 20:19:29 GMT  
		Size: 18.8 MB (18759919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320b93d95aa1cf3f1430c41fd73db6dbce1a9555be411bdc7b8beb2ccd712412`  
		Last Modified: Tue, 23 Aug 2022 20:19:25 GMT  
		Size: 2.9 KB (2903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9afae3dc366acd2e94f54c7ed688bad5b07e398c1d0b98d1c3397adbc3d1b55c`  
		Last Modified: Tue, 23 Aug 2022 20:20:07 GMT  
		Size: 41.8 MB (41849146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c6f4c95ed83df0120941707276fe29656a520a3f740d6ec95b730fb3232927`  
		Last Modified: Tue, 23 Aug 2022 20:20:00 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:f36be7242e755524990f0674ad2b66a7dc0124ab88af04d030a583e5f92c7754
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121925706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:745c4039868708153fbdf9e81a24218fa03d09a03a402c3ece548b1bdbb4c561`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:43 GMT
ADD file:21190c24a038c3c9de64b88797bf00e4c4319bd598c7c465cab2ca88d0502416 in / 
# Tue, 23 Aug 2022 01:42:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:59:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:00:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 24 Aug 2022 17:14:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 17:14:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 24 Aug 2022 17:14:34 GMT
ENV TELEGRAF_VERSION=1.23.4
# Wed, 24 Aug 2022 17:14:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 24 Aug 2022 17:14:40 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 24 Aug 2022 17:14:40 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 24 Aug 2022 17:14:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Aug 2022 17:14:40 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:c715a126a4d5182c28d2d7b1c81de847bfbbacf6851819fef3eb28e3feb7db0e`  
		Last Modified: Tue, 23 Aug 2022 01:49:30 GMT  
		Size: 50.2 MB (50204931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cecc62e275236714359bda7d1f9c8412e8fa8539f3ef682eebd9c77986c927d`  
		Last Modified: Tue, 23 Aug 2022 13:11:58 GMT  
		Size: 4.9 MB (4930827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818eb872fe75602d611beeac0db63da0a4d8a67aee8b909d5114814f76446a5e`  
		Last Modified: Tue, 23 Aug 2022 13:11:59 GMT  
		Size: 10.2 MB (10217900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28127e82dbad78eb691a0fb5e5374c2f1c2c7d4f9826ef923493608b5b98fb3c`  
		Last Modified: Wed, 24 Aug 2022 17:15:12 GMT  
		Size: 17.5 MB (17462272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a8e2427f6ebb3290b16701a3683670b1b092f3fb657747570316664b57f8e0`  
		Last Modified: Wed, 24 Aug 2022 17:15:08 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cf92227e9efb3763f04d95fc8533d16d44f5e9ff62208aae4f9e523a4ecde4`  
		Last Modified: Wed, 24 Aug 2022 17:15:51 GMT  
		Size: 39.1 MB (39106545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9db4b7aa12e76db182caeb235e71cf186e75e64e6aab4f475cf324cc43b61d`  
		Last Modified: Wed, 24 Aug 2022 17:15:44 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:a8ddacdc65a521e49f009f6771d55db2193e00f99ff5cba645e5c71ca0b50578
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125708649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66153c6da3e29fe92c650407126babd7a3446c9379a0f807b70d3693ebcb156d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:16 GMT
ADD file:ce6014a27d18915dc6d46c5c1f0f894f0027d1e41fbebb1599c16371b7bab2f1 in / 
# Tue, 23 Aug 2022 01:52:18 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:27:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 21:31:59 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 21:32:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 23 Aug 2022 21:32:29 GMT
ENV TELEGRAF_VERSION=1.23.4
# Tue, 23 Aug 2022 21:32:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 23 Aug 2022 21:32:35 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 23 Aug 2022 21:32:37 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 23 Aug 2022 21:32:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 Aug 2022 21:32:38 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:cd84405c8b9e7a8c3d580c2148d25120dd697ea61e1cb55a62f33e67988b7043`  
		Last Modified: Tue, 23 Aug 2022 01:57:29 GMT  
		Size: 53.7 MB (53690830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d98e120b809269e56de468d2b91569789c521011e4d9b1806e43fd04462de2`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 4.9 MB (4944180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb6be5911b40ca548e48c10b09cb2312f1698b4c84f09711c69389a94b1a8be`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 10.7 MB (10657442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab23840b45319a569927bb1e754dbbc4a1cd2644adaf7e32337156a0d803b491`  
		Last Modified: Tue, 23 Aug 2022 21:33:03 GMT  
		Size: 18.4 MB (18382761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8209f5a5eb7e11a25b57321f7e44a027d4c987c6abce3e24edf37b2184eb729`  
		Last Modified: Tue, 23 Aug 2022 21:33:00 GMT  
		Size: 2.9 KB (2858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e18d77d74c012eeac46b242bc3673fc10630818bb08c4fdef95a6ecb2b33767`  
		Last Modified: Tue, 23 Aug 2022 21:33:39 GMT  
		Size: 38.0 MB (38030233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e9a4598baf2ed832676e49bb46f60f62fe677ce35e2a18ce5cb976566e3863`  
		Last Modified: Tue, 23 Aug 2022 21:33:33 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.23-alpine`

```console
$ docker pull telegraf@sha256:04720ca0cd1c6740654e118cb52aa321f22cd48895c69315f320217e9f2e8f1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.23-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:010b7540eef21edeabc6330b8d0356f6375576f15fe048ac6625bff3a8a85755
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47899337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd9d6a1dd2db21ee7d8ac8b11297ef4ba1800b86e3ee9943511a3bbc770c1685`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:22:56 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 10 Aug 2022 01:22:58 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 17 Aug 2022 00:33:57 GMT
ENV TELEGRAF_VERSION=1.23.4
# Wed, 17 Aug 2022 00:34:04 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 17 Aug 2022 00:34:05 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 17 Aug 2022 00:34:05 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 17 Aug 2022 00:34:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Aug 2022 00:34:05 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b6e02c851cec1d59f28ff9497d3672a3b33ce39a9edb228b5744eb93372150`  
		Last Modified: Wed, 10 Aug 2022 01:23:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef163f69f1d36aa05f1f04751bf3169514539aa167c9094972f9987642270aab`  
		Last Modified: Wed, 10 Aug 2022 01:23:53 GMT  
		Size: 3.4 MB (3387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132a81449ba98f0e93f10ea3080cf2a9fa996d7affd65aad4434f51d51be9ecb`  
		Last Modified: Wed, 17 Aug 2022 00:34:55 GMT  
		Size: 41.7 MB (41687422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568f020258e07d85c657dec82908bc87f4f7765639c1bf5bd3ba49501157b064`  
		Last Modified: Wed, 17 Aug 2022 00:34:48 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.23.4`

```console
$ docker pull telegraf@sha256:b2afad2ff2bb5b155d3ecc9f7037c51d9f505f535d1bc2569d625725ee3f8b2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.23.4` - linux; amd64

```console
$ docker pull telegraf@sha256:6579540446d8b48a68ee70a5d00aec0180a394b390f5c274192c125498befe80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131659359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7b77eb6d0523c0d58a999fb389e9023a81544aa60e91cd318e6d8d8d48240d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:48:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 20:18:39 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 20:18:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 23 Aug 2022 20:18:59 GMT
ENV TELEGRAF_VERSION=1.23.4
# Tue, 23 Aug 2022 20:19:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 23 Aug 2022 20:19:03 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 23 Aug 2022 20:19:04 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 23 Aug 2022 20:19:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 Aug 2022 20:19:04 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e94d13e55e7a4ef17ff21376f57fb95c7e1706931f8704aa99260968d81f6e4`  
		Last Modified: Tue, 23 Aug 2022 00:55:37 GMT  
		Size: 5.2 MB (5163019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9c7528c685216129e8e67bf362a7702e7b1daa585ab85546a41508830657d6`  
		Last Modified: Tue, 23 Aug 2022 00:55:38 GMT  
		Size: 10.9 MB (10876472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bf78e724b533506c47d613e8c51e7756df404678ac937fb012ecd677818fe8`  
		Last Modified: Tue, 23 Aug 2022 20:19:29 GMT  
		Size: 18.8 MB (18759919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320b93d95aa1cf3f1430c41fd73db6dbce1a9555be411bdc7b8beb2ccd712412`  
		Last Modified: Tue, 23 Aug 2022 20:19:25 GMT  
		Size: 2.9 KB (2903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9afae3dc366acd2e94f54c7ed688bad5b07e398c1d0b98d1c3397adbc3d1b55c`  
		Last Modified: Tue, 23 Aug 2022 20:20:07 GMT  
		Size: 41.8 MB (41849146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c6f4c95ed83df0120941707276fe29656a520a3f740d6ec95b730fb3232927`  
		Last Modified: Tue, 23 Aug 2022 20:20:00 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23.4` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:f36be7242e755524990f0674ad2b66a7dc0124ab88af04d030a583e5f92c7754
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121925706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:745c4039868708153fbdf9e81a24218fa03d09a03a402c3ece548b1bdbb4c561`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:43 GMT
ADD file:21190c24a038c3c9de64b88797bf00e4c4319bd598c7c465cab2ca88d0502416 in / 
# Tue, 23 Aug 2022 01:42:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:59:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:00:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 24 Aug 2022 17:14:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 17:14:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 24 Aug 2022 17:14:34 GMT
ENV TELEGRAF_VERSION=1.23.4
# Wed, 24 Aug 2022 17:14:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 24 Aug 2022 17:14:40 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 24 Aug 2022 17:14:40 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 24 Aug 2022 17:14:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Aug 2022 17:14:40 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:c715a126a4d5182c28d2d7b1c81de847bfbbacf6851819fef3eb28e3feb7db0e`  
		Last Modified: Tue, 23 Aug 2022 01:49:30 GMT  
		Size: 50.2 MB (50204931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cecc62e275236714359bda7d1f9c8412e8fa8539f3ef682eebd9c77986c927d`  
		Last Modified: Tue, 23 Aug 2022 13:11:58 GMT  
		Size: 4.9 MB (4930827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818eb872fe75602d611beeac0db63da0a4d8a67aee8b909d5114814f76446a5e`  
		Last Modified: Tue, 23 Aug 2022 13:11:59 GMT  
		Size: 10.2 MB (10217900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28127e82dbad78eb691a0fb5e5374c2f1c2c7d4f9826ef923493608b5b98fb3c`  
		Last Modified: Wed, 24 Aug 2022 17:15:12 GMT  
		Size: 17.5 MB (17462272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a8e2427f6ebb3290b16701a3683670b1b092f3fb657747570316664b57f8e0`  
		Last Modified: Wed, 24 Aug 2022 17:15:08 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cf92227e9efb3763f04d95fc8533d16d44f5e9ff62208aae4f9e523a4ecde4`  
		Last Modified: Wed, 24 Aug 2022 17:15:51 GMT  
		Size: 39.1 MB (39106545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9db4b7aa12e76db182caeb235e71cf186e75e64e6aab4f475cf324cc43b61d`  
		Last Modified: Wed, 24 Aug 2022 17:15:44 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23.4` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:a8ddacdc65a521e49f009f6771d55db2193e00f99ff5cba645e5c71ca0b50578
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125708649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66153c6da3e29fe92c650407126babd7a3446c9379a0f807b70d3693ebcb156d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:16 GMT
ADD file:ce6014a27d18915dc6d46c5c1f0f894f0027d1e41fbebb1599c16371b7bab2f1 in / 
# Tue, 23 Aug 2022 01:52:18 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:27:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 21:31:59 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 21:32:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 23 Aug 2022 21:32:29 GMT
ENV TELEGRAF_VERSION=1.23.4
# Tue, 23 Aug 2022 21:32:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 23 Aug 2022 21:32:35 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 23 Aug 2022 21:32:37 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 23 Aug 2022 21:32:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 Aug 2022 21:32:38 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:cd84405c8b9e7a8c3d580c2148d25120dd697ea61e1cb55a62f33e67988b7043`  
		Last Modified: Tue, 23 Aug 2022 01:57:29 GMT  
		Size: 53.7 MB (53690830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d98e120b809269e56de468d2b91569789c521011e4d9b1806e43fd04462de2`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 4.9 MB (4944180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb6be5911b40ca548e48c10b09cb2312f1698b4c84f09711c69389a94b1a8be`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 10.7 MB (10657442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab23840b45319a569927bb1e754dbbc4a1cd2644adaf7e32337156a0d803b491`  
		Last Modified: Tue, 23 Aug 2022 21:33:03 GMT  
		Size: 18.4 MB (18382761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8209f5a5eb7e11a25b57321f7e44a027d4c987c6abce3e24edf37b2184eb729`  
		Last Modified: Tue, 23 Aug 2022 21:33:00 GMT  
		Size: 2.9 KB (2858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e18d77d74c012eeac46b242bc3673fc10630818bb08c4fdef95a6ecb2b33767`  
		Last Modified: Tue, 23 Aug 2022 21:33:39 GMT  
		Size: 38.0 MB (38030233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e9a4598baf2ed832676e49bb46f60f62fe677ce35e2a18ce5cb976566e3863`  
		Last Modified: Tue, 23 Aug 2022 21:33:33 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.23.4-alpine`

```console
$ docker pull telegraf@sha256:04720ca0cd1c6740654e118cb52aa321f22cd48895c69315f320217e9f2e8f1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.23.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:010b7540eef21edeabc6330b8d0356f6375576f15fe048ac6625bff3a8a85755
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47899337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd9d6a1dd2db21ee7d8ac8b11297ef4ba1800b86e3ee9943511a3bbc770c1685`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:22:56 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 10 Aug 2022 01:22:58 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 17 Aug 2022 00:33:57 GMT
ENV TELEGRAF_VERSION=1.23.4
# Wed, 17 Aug 2022 00:34:04 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 17 Aug 2022 00:34:05 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 17 Aug 2022 00:34:05 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 17 Aug 2022 00:34:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Aug 2022 00:34:05 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b6e02c851cec1d59f28ff9497d3672a3b33ce39a9edb228b5744eb93372150`  
		Last Modified: Wed, 10 Aug 2022 01:23:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef163f69f1d36aa05f1f04751bf3169514539aa167c9094972f9987642270aab`  
		Last Modified: Wed, 10 Aug 2022 01:23:53 GMT  
		Size: 3.4 MB (3387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132a81449ba98f0e93f10ea3080cf2a9fa996d7affd65aad4434f51d51be9ecb`  
		Last Modified: Wed, 17 Aug 2022 00:34:55 GMT  
		Size: 41.7 MB (41687422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568f020258e07d85c657dec82908bc87f4f7765639c1bf5bd3ba49501157b064`  
		Last Modified: Wed, 17 Aug 2022 00:34:48 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.24`

**does not exist** (yet?)

## `telegraf:1.24-alpine`

**does not exist** (yet?)

## `telegraf:1.24.0`

**does not exist** (yet?)

## `telegraf:1.24.0-alpine`

**does not exist** (yet?)

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:04720ca0cd1c6740654e118cb52aa321f22cd48895c69315f320217e9f2e8f1b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:010b7540eef21edeabc6330b8d0356f6375576f15fe048ac6625bff3a8a85755
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47899337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd9d6a1dd2db21ee7d8ac8b11297ef4ba1800b86e3ee9943511a3bbc770c1685`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 01:22:56 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 10 Aug 2022 01:22:58 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 17 Aug 2022 00:33:57 GMT
ENV TELEGRAF_VERSION=1.23.4
# Wed, 17 Aug 2022 00:34:04 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 17 Aug 2022 00:34:05 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 17 Aug 2022 00:34:05 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 17 Aug 2022 00:34:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 17 Aug 2022 00:34:05 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b6e02c851cec1d59f28ff9497d3672a3b33ce39a9edb228b5744eb93372150`  
		Last Modified: Wed, 10 Aug 2022 01:23:53 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef163f69f1d36aa05f1f04751bf3169514539aa167c9094972f9987642270aab`  
		Last Modified: Wed, 10 Aug 2022 01:23:53 GMT  
		Size: 3.4 MB (3387922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132a81449ba98f0e93f10ea3080cf2a9fa996d7affd65aad4434f51d51be9ecb`  
		Last Modified: Wed, 17 Aug 2022 00:34:55 GMT  
		Size: 41.7 MB (41687422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:568f020258e07d85c657dec82908bc87f4f7765639c1bf5bd3ba49501157b064`  
		Last Modified: Wed, 17 Aug 2022 00:34:48 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:b2afad2ff2bb5b155d3ecc9f7037c51d9f505f535d1bc2569d625725ee3f8b2b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:6579540446d8b48a68ee70a5d00aec0180a394b390f5c274192c125498befe80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131659359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7b77eb6d0523c0d58a999fb389e9023a81544aa60e91cd318e6d8d8d48240d7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:40 GMT
ADD file:6944d322f4c04bd2192061822af5cbec8ac0a6b424c461d66174d32aed604972 in / 
# Tue, 23 Aug 2022 00:20:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:48:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:48:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 20:18:39 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 20:18:41 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 23 Aug 2022 20:18:59 GMT
ENV TELEGRAF_VERSION=1.23.4
# Tue, 23 Aug 2022 20:19:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 23 Aug 2022 20:19:03 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 23 Aug 2022 20:19:04 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 23 Aug 2022 20:19:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 Aug 2022 20:19:04 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:1671565cc8df8c365c9b661d3fbc164e73d01f1b0430c6179588428f99a9da2e`  
		Last Modified: Tue, 23 Aug 2022 00:24:32 GMT  
		Size: 55.0 MB (55007555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e94d13e55e7a4ef17ff21376f57fb95c7e1706931f8704aa99260968d81f6e4`  
		Last Modified: Tue, 23 Aug 2022 00:55:37 GMT  
		Size: 5.2 MB (5163019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9c7528c685216129e8e67bf362a7702e7b1daa585ab85546a41508830657d6`  
		Last Modified: Tue, 23 Aug 2022 00:55:38 GMT  
		Size: 10.9 MB (10876472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75bf78e724b533506c47d613e8c51e7756df404678ac937fb012ecd677818fe8`  
		Last Modified: Tue, 23 Aug 2022 20:19:29 GMT  
		Size: 18.8 MB (18759919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320b93d95aa1cf3f1430c41fd73db6dbce1a9555be411bdc7b8beb2ccd712412`  
		Last Modified: Tue, 23 Aug 2022 20:19:25 GMT  
		Size: 2.9 KB (2903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9afae3dc366acd2e94f54c7ed688bad5b07e398c1d0b98d1c3397adbc3d1b55c`  
		Last Modified: Tue, 23 Aug 2022 20:20:07 GMT  
		Size: 41.8 MB (41849146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c6f4c95ed83df0120941707276fe29656a520a3f740d6ec95b730fb3232927`  
		Last Modified: Tue, 23 Aug 2022 20:20:00 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:f36be7242e755524990f0674ad2b66a7dc0124ab88af04d030a583e5f92c7754
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121925706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:745c4039868708153fbdf9e81a24218fa03d09a03a402c3ece548b1bdbb4c561`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 Aug 2022 01:42:43 GMT
ADD file:21190c24a038c3c9de64b88797bf00e4c4319bd598c7c465cab2ca88d0502416 in / 
# Tue, 23 Aug 2022 01:42:43 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 12:59:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:00:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 24 Aug 2022 17:14:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 24 Aug 2022 17:14:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 24 Aug 2022 17:14:34 GMT
ENV TELEGRAF_VERSION=1.23.4
# Wed, 24 Aug 2022 17:14:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 24 Aug 2022 17:14:40 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 24 Aug 2022 17:14:40 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 24 Aug 2022 17:14:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 24 Aug 2022 17:14:40 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:c715a126a4d5182c28d2d7b1c81de847bfbbacf6851819fef3eb28e3feb7db0e`  
		Last Modified: Tue, 23 Aug 2022 01:49:30 GMT  
		Size: 50.2 MB (50204931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cecc62e275236714359bda7d1f9c8412e8fa8539f3ef682eebd9c77986c927d`  
		Last Modified: Tue, 23 Aug 2022 13:11:58 GMT  
		Size: 4.9 MB (4930827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818eb872fe75602d611beeac0db63da0a4d8a67aee8b909d5114814f76446a5e`  
		Last Modified: Tue, 23 Aug 2022 13:11:59 GMT  
		Size: 10.2 MB (10217900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28127e82dbad78eb691a0fb5e5374c2f1c2c7d4f9826ef923493608b5b98fb3c`  
		Last Modified: Wed, 24 Aug 2022 17:15:12 GMT  
		Size: 17.5 MB (17462272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a8e2427f6ebb3290b16701a3683670b1b092f3fb657747570316664b57f8e0`  
		Last Modified: Wed, 24 Aug 2022 17:15:08 GMT  
		Size: 2.9 KB (2886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cf92227e9efb3763f04d95fc8533d16d44f5e9ff62208aae4f9e523a4ecde4`  
		Last Modified: Wed, 24 Aug 2022 17:15:51 GMT  
		Size: 39.1 MB (39106545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9db4b7aa12e76db182caeb235e71cf186e75e64e6aab4f475cf324cc43b61d`  
		Last Modified: Wed, 24 Aug 2022 17:15:44 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:a8ddacdc65a521e49f009f6771d55db2193e00f99ff5cba645e5c71ca0b50578
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.7 MB (125708649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66153c6da3e29fe92c650407126babd7a3446c9379a0f807b70d3693ebcb156d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:16 GMT
ADD file:ce6014a27d18915dc6d46c5c1f0f894f0027d1e41fbebb1599c16371b7bab2f1 in / 
# Tue, 23 Aug 2022 01:52:18 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:27:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 21:31:59 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 21:32:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 23 Aug 2022 21:32:29 GMT
ENV TELEGRAF_VERSION=1.23.4
# Tue, 23 Aug 2022 21:32:34 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 23 Aug 2022 21:32:35 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 23 Aug 2022 21:32:37 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 23 Aug 2022 21:32:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 23 Aug 2022 21:32:38 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:cd84405c8b9e7a8c3d580c2148d25120dd697ea61e1cb55a62f33e67988b7043`  
		Last Modified: Tue, 23 Aug 2022 01:57:29 GMT  
		Size: 53.7 MB (53690830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d98e120b809269e56de468d2b91569789c521011e4d9b1806e43fd04462de2`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 4.9 MB (4944180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb6be5911b40ca548e48c10b09cb2312f1698b4c84f09711c69389a94b1a8be`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 10.7 MB (10657442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab23840b45319a569927bb1e754dbbc4a1cd2644adaf7e32337156a0d803b491`  
		Last Modified: Tue, 23 Aug 2022 21:33:03 GMT  
		Size: 18.4 MB (18382761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8209f5a5eb7e11a25b57321f7e44a027d4c987c6abce3e24edf37b2184eb729`  
		Last Modified: Tue, 23 Aug 2022 21:33:00 GMT  
		Size: 2.9 KB (2858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e18d77d74c012eeac46b242bc3673fc10630818bb08c4fdef95a6ecb2b33767`  
		Last Modified: Tue, 23 Aug 2022 21:33:39 GMT  
		Size: 38.0 MB (38030233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e9a4598baf2ed832676e49bb46f60f62fe677ce35e2a18ce5cb976566e3863`  
		Last Modified: Tue, 23 Aug 2022 21:33:33 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
