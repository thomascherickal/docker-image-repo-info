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
-	[`telegraf:1.27.4`](#telegraf1274)
-	[`telegraf:1.27.4-alpine`](#telegraf1274-alpine)
-	[`telegraf:alpine`](#telegrafalpine)
-	[`telegraf:latest`](#telegraflatest)

## `telegraf:1.25`

```console
$ docker pull telegraf@sha256:af3c122d4e79fea0fccaad14c7abbf3c14845f09e12a11563e94a7bb500e05ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.25` - linux; amd64

```console
$ docker pull telegraf@sha256:c2d2494320359017faa9405cbe8acdb981ef68dcf35a3e8138113d4a807b3985
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.2 MB (136155922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f572ae13354b3d928ee794c244a4462ef3df9e7f55f868877f20e2f42c51b293`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:59:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 00:54:51 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 00:54:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Aug 2023 00:54:52 GMT
ENV TELEGRAF_VERSION=1.25.3
# Thu, 17 Aug 2023 00:54:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 17 Aug 2023 00:54:57 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 17 Aug 2023 00:54:57 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 17 Aug 2023 00:54:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Aug 2023 00:54:57 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb4221e2c63c35bb16b63f6d24c104c7ea5d453997636c2244b66884f540537`  
		Last Modified: Wed, 16 Aug 2023 07:13:46 GMT  
		Size: 15.8 MB (15760534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1ea4dcbb3e9317fe08a2c3c94e18cb14548f0812d95e416c11f6b74cbcd099`  
		Last Modified: Thu, 17 Aug 2023 00:55:49 GMT  
		Size: 18.8 MB (18760016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaed78a4892af6a865dbc80ee77c06fb1e3a653ddad4c1000dadbd76e27324ba`  
		Last Modified: Thu, 17 Aug 2023 00:55:46 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00fd3d39302dea4d62f113b059ddc5ab87c3141ab7c3b61e4ae3db4003774d0`  
		Last Modified: Thu, 17 Aug 2023 00:55:53 GMT  
		Size: 46.6 MB (46576606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e2efb3758d7bcd6662c961d416a144fa9d92ebba341cc3eaff1ac23ce8b2ae`  
		Last Modified: Thu, 17 Aug 2023 00:55:46 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:0327cd9c4cd47fe837d50fdc4040872c8bd70db8177449506d94204a50c63078
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125936765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0b31287f04840f0b625af89374cb2d7f76f03b4f4e9c467327d9c86305d874e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:21 GMT
ADD file:b529de8b48c1e507ad6f29320c3c5cd83d8d06fa66e8d89bb62faff62700e9f2 in / 
# Wed, 16 Aug 2023 00:17:22 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:30:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 21:45:34 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 21:45:36 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Aug 2023 21:45:36 GMT
ENV TELEGRAF_VERSION=1.25.3
# Wed, 16 Aug 2023 21:45:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 16 Aug 2023 21:45:43 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 16 Aug 2023 21:45:43 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 16 Aug 2023 21:45:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Aug 2023 21:45:43 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:c53151c23650f086e15d3652b8a931fb4623765c0112e8adc74eb8853c8c9232`  
		Last Modified: Wed, 16 Aug 2023 00:21:46 GMT  
		Size: 50.2 MB (50219496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbe9a81a850f9760477ffa3083b63d636090316a05f81146ffd62a60638926a`  
		Last Modified: Wed, 16 Aug 2023 05:48:44 GMT  
		Size: 14.9 MB (14868833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119a15c02ecd117b4d86ba23a5908f78af6e8bdcb72f0f8e2af09953491510dc`  
		Last Modified: Wed, 16 Aug 2023 21:46:32 GMT  
		Size: 17.5 MB (17462350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8c72ee3df03976cc4b562fd3122851cf0ef526cf710e2da2b98bfdcbf5c4af`  
		Last Modified: Wed, 16 Aug 2023 21:46:28 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c627c315f00ac353d67ddbc32e2d8961cac7a09de489c742f45fa02edd0156`  
		Last Modified: Wed, 16 Aug 2023 21:46:36 GMT  
		Size: 43.4 MB (43383937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974c436284adbaf14bc865c0b34cf5ffadf33edce6c4852123205998347e402b`  
		Last Modified: Wed, 16 Aug 2023 21:46:28 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:8e1fee1f7fb1054915bebf315025eea8091fd4cbbabdab1f5e0f5416df281239
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130367269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4846c9e0fa31673904be7ff46b80a5d9abe0c23163335e1952cece1044da48ff`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:23:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 22:59:24 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 22:59:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Aug 2023 22:59:25 GMT
ENV TELEGRAF_VERSION=1.25.3
# Wed, 16 Aug 2023 22:59:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 16 Aug 2023 22:59:31 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 16 Aug 2023 22:59:31 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 16 Aug 2023 22:59:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Aug 2023 22:59:31 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abd0588cbb35597a784666f0dc97746829b8b4b730b73e8781fb90678ffef22`  
		Last Modified: Wed, 16 Aug 2023 01:39:26 GMT  
		Size: 15.7 MB (15746520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0860da3b4f04723a9d4c9a268a331f9cd407a2a50285086571c81082d1783d6`  
		Last Modified: Wed, 16 Aug 2023 23:00:23 GMT  
		Size: 18.6 MB (18598594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47feb01a6b330f394b7cf3a0f298b706257fb49472dfce456b10c5829246920`  
		Last Modified: Wed, 16 Aug 2023 23:00:20 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ed2d5055b7a55c3adb3c70b1f39041496545484a6a5b2f24fc8458367af3bd`  
		Last Modified: Wed, 16 Aug 2023 23:00:25 GMT  
		Size: 42.3 MB (42315221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddb3c42ceca3b41357f133ad7e2d51d0fba98bae7fde5a7683f95f91bd6ee2d`  
		Last Modified: Wed, 16 Aug 2023 23:00:20 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25-alpine`

```console
$ docker pull telegraf@sha256:117f74f4f58351a5d3f430a59c39032b14b0968532ee7e57d6f1c951b9a68620
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.25-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:090d9c6ab66f49ce2ee900a400b12772072654981816ee3cb9d7b99a4bfdb5d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52443663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cad90446844a1d6169b55f534b7ebbc7e2a184ea07f3e93e65cc04b5665ab00`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:04:25 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 09 Aug 2023 04:04:25 GMT
ENV TELEGRAF_VERSION=1.25.3
# Wed, 09 Aug 2023 04:04:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 09 Aug 2023 04:04:35 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 09 Aug 2023 04:04:35 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 09 Aug 2023 04:04:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:04:35 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81f19a7d917a9734911b177e41983aa98776e1138b57753de6adba42dd022ba`  
		Last Modified: Wed, 09 Aug 2023 04:05:25 GMT  
		Size: 2.7 MB (2671751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c696e7d69bdbeeb40d0c7f1ff4562b7d85912496041be3a50836d69dfcf6c5b`  
		Last Modified: Wed, 09 Aug 2023 04:05:32 GMT  
		Size: 46.4 MB (46392696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bcf5f4ad2a2386d9e545464cc39334e5140cd5525b726bad619116dfa9375c`  
		Last Modified: Wed, 09 Aug 2023 04:05:25 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25.3`

```console
$ docker pull telegraf@sha256:af3c122d4e79fea0fccaad14c7abbf3c14845f09e12a11563e94a7bb500e05ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.25.3` - linux; amd64

```console
$ docker pull telegraf@sha256:c2d2494320359017faa9405cbe8acdb981ef68dcf35a3e8138113d4a807b3985
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.2 MB (136155922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f572ae13354b3d928ee794c244a4462ef3df9e7f55f868877f20e2f42c51b293`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:59:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 00:54:51 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 00:54:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Aug 2023 00:54:52 GMT
ENV TELEGRAF_VERSION=1.25.3
# Thu, 17 Aug 2023 00:54:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 17 Aug 2023 00:54:57 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 17 Aug 2023 00:54:57 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 17 Aug 2023 00:54:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Aug 2023 00:54:57 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb4221e2c63c35bb16b63f6d24c104c7ea5d453997636c2244b66884f540537`  
		Last Modified: Wed, 16 Aug 2023 07:13:46 GMT  
		Size: 15.8 MB (15760534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1ea4dcbb3e9317fe08a2c3c94e18cb14548f0812d95e416c11f6b74cbcd099`  
		Last Modified: Thu, 17 Aug 2023 00:55:49 GMT  
		Size: 18.8 MB (18760016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaed78a4892af6a865dbc80ee77c06fb1e3a653ddad4c1000dadbd76e27324ba`  
		Last Modified: Thu, 17 Aug 2023 00:55:46 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00fd3d39302dea4d62f113b059ddc5ab87c3141ab7c3b61e4ae3db4003774d0`  
		Last Modified: Thu, 17 Aug 2023 00:55:53 GMT  
		Size: 46.6 MB (46576606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e2efb3758d7bcd6662c961d416a144fa9d92ebba341cc3eaff1ac23ce8b2ae`  
		Last Modified: Thu, 17 Aug 2023 00:55:46 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25.3` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:0327cd9c4cd47fe837d50fdc4040872c8bd70db8177449506d94204a50c63078
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.9 MB (125936765 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0b31287f04840f0b625af89374cb2d7f76f03b4f4e9c467327d9c86305d874e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:21 GMT
ADD file:b529de8b48c1e507ad6f29320c3c5cd83d8d06fa66e8d89bb62faff62700e9f2 in / 
# Wed, 16 Aug 2023 00:17:22 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:30:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 21:45:34 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 21:45:36 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Aug 2023 21:45:36 GMT
ENV TELEGRAF_VERSION=1.25.3
# Wed, 16 Aug 2023 21:45:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 16 Aug 2023 21:45:43 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 16 Aug 2023 21:45:43 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 16 Aug 2023 21:45:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Aug 2023 21:45:43 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:c53151c23650f086e15d3652b8a931fb4623765c0112e8adc74eb8853c8c9232`  
		Last Modified: Wed, 16 Aug 2023 00:21:46 GMT  
		Size: 50.2 MB (50219496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbe9a81a850f9760477ffa3083b63d636090316a05f81146ffd62a60638926a`  
		Last Modified: Wed, 16 Aug 2023 05:48:44 GMT  
		Size: 14.9 MB (14868833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119a15c02ecd117b4d86ba23a5908f78af6e8bdcb72f0f8e2af09953491510dc`  
		Last Modified: Wed, 16 Aug 2023 21:46:32 GMT  
		Size: 17.5 MB (17462350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8c72ee3df03976cc4b562fd3122851cf0ef526cf710e2da2b98bfdcbf5c4af`  
		Last Modified: Wed, 16 Aug 2023 21:46:28 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c627c315f00ac353d67ddbc32e2d8961cac7a09de489c742f45fa02edd0156`  
		Last Modified: Wed, 16 Aug 2023 21:46:36 GMT  
		Size: 43.4 MB (43383937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:974c436284adbaf14bc865c0b34cf5ffadf33edce6c4852123205998347e402b`  
		Last Modified: Wed, 16 Aug 2023 21:46:28 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25.3` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:8e1fee1f7fb1054915bebf315025eea8091fd4cbbabdab1f5e0f5416df281239
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130367269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4846c9e0fa31673904be7ff46b80a5d9abe0c23163335e1952cece1044da48ff`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:23:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 22:59:24 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 22:59:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Aug 2023 22:59:25 GMT
ENV TELEGRAF_VERSION=1.25.3
# Wed, 16 Aug 2023 22:59:30 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 16 Aug 2023 22:59:31 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 16 Aug 2023 22:59:31 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 16 Aug 2023 22:59:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Aug 2023 22:59:31 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abd0588cbb35597a784666f0dc97746829b8b4b730b73e8781fb90678ffef22`  
		Last Modified: Wed, 16 Aug 2023 01:39:26 GMT  
		Size: 15.7 MB (15746520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0860da3b4f04723a9d4c9a268a331f9cd407a2a50285086571c81082d1783d6`  
		Last Modified: Wed, 16 Aug 2023 23:00:23 GMT  
		Size: 18.6 MB (18598594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47feb01a6b330f394b7cf3a0f298b706257fb49472dfce456b10c5829246920`  
		Last Modified: Wed, 16 Aug 2023 23:00:20 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ed2d5055b7a55c3adb3c70b1f39041496545484a6a5b2f24fc8458367af3bd`  
		Last Modified: Wed, 16 Aug 2023 23:00:25 GMT  
		Size: 42.3 MB (42315221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eddb3c42ceca3b41357f133ad7e2d51d0fba98bae7fde5a7683f95f91bd6ee2d`  
		Last Modified: Wed, 16 Aug 2023 23:00:20 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25.3-alpine`

```console
$ docker pull telegraf@sha256:117f74f4f58351a5d3f430a59c39032b14b0968532ee7e57d6f1c951b9a68620
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.25.3-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:090d9c6ab66f49ce2ee900a400b12772072654981816ee3cb9d7b99a4bfdb5d6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52443663 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cad90446844a1d6169b55f534b7ebbc7e2a184ea07f3e93e65cc04b5665ab00`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:04:25 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 09 Aug 2023 04:04:25 GMT
ENV TELEGRAF_VERSION=1.25.3
# Wed, 09 Aug 2023 04:04:35 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 09 Aug 2023 04:04:35 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 09 Aug 2023 04:04:35 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 09 Aug 2023 04:04:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:04:35 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81f19a7d917a9734911b177e41983aa98776e1138b57753de6adba42dd022ba`  
		Last Modified: Wed, 09 Aug 2023 04:05:25 GMT  
		Size: 2.7 MB (2671751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c696e7d69bdbeeb40d0c7f1ff4562b7d85912496041be3a50836d69dfcf6c5b`  
		Last Modified: Wed, 09 Aug 2023 04:05:32 GMT  
		Size: 46.4 MB (46392696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bcf5f4ad2a2386d9e545464cc39334e5140cd5525b726bad619116dfa9375c`  
		Last Modified: Wed, 09 Aug 2023 04:05:25 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26`

```console
$ docker pull telegraf@sha256:f2d58e185ceef3588635fd91427bf6d1cb0e807949099586eba31bec940b1011
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.26` - linux; amd64

```console
$ docker pull telegraf@sha256:74425a03d033a9d5731af8d27f35fbf32b6598ea0bae00731ed6197635ed34e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140131816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:132b77fefeb90d518943b8c36d30ca76812620637e6fa471706c5c9c091eba35`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:59:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 00:54:51 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 00:54:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Aug 2023 00:55:03 GMT
ENV TELEGRAF_VERSION=1.26.3
# Thu, 17 Aug 2023 00:55:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 17 Aug 2023 00:55:09 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 17 Aug 2023 00:55:09 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 17 Aug 2023 00:55:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Aug 2023 00:55:09 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb4221e2c63c35bb16b63f6d24c104c7ea5d453997636c2244b66884f540537`  
		Last Modified: Wed, 16 Aug 2023 07:13:46 GMT  
		Size: 15.8 MB (15760534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1ea4dcbb3e9317fe08a2c3c94e18cb14548f0812d95e416c11f6b74cbcd099`  
		Last Modified: Thu, 17 Aug 2023 00:55:49 GMT  
		Size: 18.8 MB (18760016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaed78a4892af6a865dbc80ee77c06fb1e3a653ddad4c1000dadbd76e27324ba`  
		Last Modified: Thu, 17 Aug 2023 00:55:46 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680691c7a2e53a7579aee59e9a7aa62537df269bcf98b26cd5ac19eb00010773`  
		Last Modified: Thu, 17 Aug 2023 00:56:11 GMT  
		Size: 50.6 MB (50552498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08939d8a7a36752ffa2373559548c244ae03ec254328384c13cbe4c4a2fd094`  
		Last Modified: Thu, 17 Aug 2023 00:56:03 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:1d1f87fd7f2a97c68a4233e8b1136371641e23022dc631716c19ddd73bb52ba2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129835549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c490d59dd22d1601c2dc8bdf1e2156b83a45b09f3904312c78e0766496f703e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:21 GMT
ADD file:b529de8b48c1e507ad6f29320c3c5cd83d8d06fa66e8d89bb62faff62700e9f2 in / 
# Wed, 16 Aug 2023 00:17:22 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:30:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 21:45:34 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 21:45:36 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Aug 2023 21:45:45 GMT
ENV TELEGRAF_VERSION=1.26.3
# Wed, 16 Aug 2023 21:45:53 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 16 Aug 2023 21:45:53 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 16 Aug 2023 21:45:53 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 16 Aug 2023 21:45:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Aug 2023 21:45:54 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:c53151c23650f086e15d3652b8a931fb4623765c0112e8adc74eb8853c8c9232`  
		Last Modified: Wed, 16 Aug 2023 00:21:46 GMT  
		Size: 50.2 MB (50219496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbe9a81a850f9760477ffa3083b63d636090316a05f81146ffd62a60638926a`  
		Last Modified: Wed, 16 Aug 2023 05:48:44 GMT  
		Size: 14.9 MB (14868833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119a15c02ecd117b4d86ba23a5908f78af6e8bdcb72f0f8e2af09953491510dc`  
		Last Modified: Wed, 16 Aug 2023 21:46:32 GMT  
		Size: 17.5 MB (17462350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8c72ee3df03976cc4b562fd3122851cf0ef526cf710e2da2b98bfdcbf5c4af`  
		Last Modified: Wed, 16 Aug 2023 21:46:28 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddb755625c933c081447bad8f5a5481c90589ba2d6e7e58282451225ab5b5ff`  
		Last Modified: Wed, 16 Aug 2023 21:46:52 GMT  
		Size: 47.3 MB (47282722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095638b85170300902f545649f900c5753504de5ec2ec3fadc02237e1b79f76b`  
		Last Modified: Wed, 16 Aug 2023 21:46:44 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:3409764a087b07d7d6a6bb2a9d6dd3492c0980763d929e6e2b27804a0e87474e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (134023919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29d166bbe02df4cbdd1ac4581d05c049c17f57106b04b95ae951e9c706b8ece3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:23:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 22:59:24 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 22:59:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Aug 2023 22:59:36 GMT
ENV TELEGRAF_VERSION=1.26.3
# Wed, 16 Aug 2023 22:59:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 16 Aug 2023 22:59:41 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 16 Aug 2023 22:59:41 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 16 Aug 2023 22:59:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Aug 2023 22:59:41 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abd0588cbb35597a784666f0dc97746829b8b4b730b73e8781fb90678ffef22`  
		Last Modified: Wed, 16 Aug 2023 01:39:26 GMT  
		Size: 15.7 MB (15746520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0860da3b4f04723a9d4c9a268a331f9cd407a2a50285086571c81082d1783d6`  
		Last Modified: Wed, 16 Aug 2023 23:00:23 GMT  
		Size: 18.6 MB (18598594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47feb01a6b330f394b7cf3a0f298b706257fb49472dfce456b10c5829246920`  
		Last Modified: Wed, 16 Aug 2023 23:00:20 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8246b58a8896f6436b2dc326660aa95429a1ca47029cc393a35b0474fc930a1`  
		Last Modified: Wed, 16 Aug 2023 23:00:39 GMT  
		Size: 46.0 MB (45971867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c23e9f404c3647a45d05473c06b1b600a221bf86ba91389c588dbd3a952eda19`  
		Last Modified: Wed, 16 Aug 2023 23:00:34 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26-alpine`

```console
$ docker pull telegraf@sha256:6324054ecb1955be213e63944c66a84a8fd98972aa93f95d116dc8c4524e5c2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.26-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:78f7670b9bcd3a4aad80c6ebbee49cf7335f6a5d2d859c953bfa64f8006f38e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.4 MB (56442923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84c98ff0b99b251029050997eaa7c7f4781b917a79b8bed512a729e69982f7c2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:04:25 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 09 Aug 2023 04:04:40 GMT
ENV TELEGRAF_VERSION=1.26.3
# Wed, 09 Aug 2023 04:04:52 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 09 Aug 2023 04:04:52 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 09 Aug 2023 04:04:52 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 09 Aug 2023 04:04:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:04:52 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81f19a7d917a9734911b177e41983aa98776e1138b57753de6adba42dd022ba`  
		Last Modified: Wed, 09 Aug 2023 04:05:25 GMT  
		Size: 2.7 MB (2671751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ffe32ffc35ea9bbf469c7313d2e28eb55dce4def6d7921b4a8ed64d5065827`  
		Last Modified: Wed, 09 Aug 2023 04:05:49 GMT  
		Size: 50.4 MB (50391957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf8ae69b2b52e8bf419120908053a720d3c85e1cd6eee473ce91f75e98b516a`  
		Last Modified: Wed, 09 Aug 2023 04:05:41 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:e663774ce831002c89534e1f287e55d3bd316713b618e67701db26fbe5d8028d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51774942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8375fdb742f718828f27c8a87bcacfe958d4efe3802049d8e0f2db47b8b63653`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 00:46:08 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:25:36 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 09 Aug 2023 04:25:36 GMT
ENV TELEGRAF_VERSION=1.26.3
# Wed, 09 Aug 2023 04:25:43 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 09 Aug 2023 04:25:44 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 09 Aug 2023 04:25:44 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 09 Aug 2023 04:25:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:25:44 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd1799839c258f2f362340c258c49aa080e354fd0e137266f54d413ef004a1b`  
		Last Modified: Wed, 09 Aug 2023 00:46:37 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47f27f99383dfe7b1872c5a815d6081f46d86eeaa05a1cb0fef13827b0fe766`  
		Last Modified: Wed, 09 Aug 2023 04:26:17 GMT  
		Size: 2.7 MB (2703763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014a294016445a25dbb6ffc116ee7cabe334d80ec4a227196a4109180dbe204b`  
		Last Modified: Wed, 09 Aug 2023 04:26:22 GMT  
		Size: 45.8 MB (45812279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8399f752cf89525b188eb16e83df90ab39e25524c9308c289d2f748445fca4`  
		Last Modified: Wed, 09 Aug 2023 04:26:16 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26.3`

```console
$ docker pull telegraf@sha256:f2d58e185ceef3588635fd91427bf6d1cb0e807949099586eba31bec940b1011
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.26.3` - linux; amd64

```console
$ docker pull telegraf@sha256:74425a03d033a9d5731af8d27f35fbf32b6598ea0bae00731ed6197635ed34e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140131816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:132b77fefeb90d518943b8c36d30ca76812620637e6fa471706c5c9c091eba35`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:57 GMT
ADD file:20f89ff93bfbd6c9fb1a97058a1f3de4485a8974e8a83892072c511fbd2e4134 in / 
# Wed, 16 Aug 2023 00:59:58 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:59:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 00:54:51 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 00:54:52 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Aug 2023 00:55:03 GMT
ENV TELEGRAF_VERSION=1.26.3
# Thu, 17 Aug 2023 00:55:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 17 Aug 2023 00:55:09 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 17 Aug 2023 00:55:09 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 17 Aug 2023 00:55:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Aug 2023 00:55:09 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:6a70103cc499a199e10e379794c60aa524d9598587cc2bdfe2995642c2da8df7`  
		Last Modified: Wed, 16 Aug 2023 01:04:50 GMT  
		Size: 55.1 MB (55056621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccb4221e2c63c35bb16b63f6d24c104c7ea5d453997636c2244b66884f540537`  
		Last Modified: Wed, 16 Aug 2023 07:13:46 GMT  
		Size: 15.8 MB (15760534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1ea4dcbb3e9317fe08a2c3c94e18cb14548f0812d95e416c11f6b74cbcd099`  
		Last Modified: Thu, 17 Aug 2023 00:55:49 GMT  
		Size: 18.8 MB (18760016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaed78a4892af6a865dbc80ee77c06fb1e3a653ddad4c1000dadbd76e27324ba`  
		Last Modified: Thu, 17 Aug 2023 00:55:46 GMT  
		Size: 1.8 KB (1804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680691c7a2e53a7579aee59e9a7aa62537df269bcf98b26cd5ac19eb00010773`  
		Last Modified: Thu, 17 Aug 2023 00:56:11 GMT  
		Size: 50.6 MB (50552498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08939d8a7a36752ffa2373559548c244ae03ec254328384c13cbe4c4a2fd094`  
		Last Modified: Thu, 17 Aug 2023 00:56:03 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26.3` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:1d1f87fd7f2a97c68a4233e8b1136371641e23022dc631716c19ddd73bb52ba2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129835549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c490d59dd22d1601c2dc8bdf1e2156b83a45b09f3904312c78e0766496f703e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:21 GMT
ADD file:b529de8b48c1e507ad6f29320c3c5cd83d8d06fa66e8d89bb62faff62700e9f2 in / 
# Wed, 16 Aug 2023 00:17:22 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:30:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 21:45:34 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 21:45:36 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Aug 2023 21:45:45 GMT
ENV TELEGRAF_VERSION=1.26.3
# Wed, 16 Aug 2023 21:45:53 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 16 Aug 2023 21:45:53 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 16 Aug 2023 21:45:53 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 16 Aug 2023 21:45:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Aug 2023 21:45:54 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:c53151c23650f086e15d3652b8a931fb4623765c0112e8adc74eb8853c8c9232`  
		Last Modified: Wed, 16 Aug 2023 00:21:46 GMT  
		Size: 50.2 MB (50219496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbe9a81a850f9760477ffa3083b63d636090316a05f81146ffd62a60638926a`  
		Last Modified: Wed, 16 Aug 2023 05:48:44 GMT  
		Size: 14.9 MB (14868833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:119a15c02ecd117b4d86ba23a5908f78af6e8bdcb72f0f8e2af09953491510dc`  
		Last Modified: Wed, 16 Aug 2023 21:46:32 GMT  
		Size: 17.5 MB (17462350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8c72ee3df03976cc4b562fd3122851cf0ef526cf710e2da2b98bfdcbf5c4af`  
		Last Modified: Wed, 16 Aug 2023 21:46:28 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ddb755625c933c081447bad8f5a5481c90589ba2d6e7e58282451225ab5b5ff`  
		Last Modified: Wed, 16 Aug 2023 21:46:52 GMT  
		Size: 47.3 MB (47282722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095638b85170300902f545649f900c5753504de5ec2ec3fadc02237e1b79f76b`  
		Last Modified: Wed, 16 Aug 2023 21:46:44 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26.3` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:3409764a087b07d7d6a6bb2a9d6dd3492c0980763d929e6e2b27804a0e87474e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (134023919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29d166bbe02df4cbdd1ac4581d05c049c17f57106b04b95ae951e9c706b8ece3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:23:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 22:59:24 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 22:59:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Aug 2023 22:59:36 GMT
ENV TELEGRAF_VERSION=1.26.3
# Wed, 16 Aug 2023 22:59:40 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 16 Aug 2023 22:59:41 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 16 Aug 2023 22:59:41 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 16 Aug 2023 22:59:41 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Aug 2023 22:59:41 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abd0588cbb35597a784666f0dc97746829b8b4b730b73e8781fb90678ffef22`  
		Last Modified: Wed, 16 Aug 2023 01:39:26 GMT  
		Size: 15.7 MB (15746520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0860da3b4f04723a9d4c9a268a331f9cd407a2a50285086571c81082d1783d6`  
		Last Modified: Wed, 16 Aug 2023 23:00:23 GMT  
		Size: 18.6 MB (18598594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47feb01a6b330f394b7cf3a0f298b706257fb49472dfce456b10c5829246920`  
		Last Modified: Wed, 16 Aug 2023 23:00:20 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8246b58a8896f6436b2dc326660aa95429a1ca47029cc393a35b0474fc930a1`  
		Last Modified: Wed, 16 Aug 2023 23:00:39 GMT  
		Size: 46.0 MB (45971867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c23e9f404c3647a45d05473c06b1b600a221bf86ba91389c588dbd3a952eda19`  
		Last Modified: Wed, 16 Aug 2023 23:00:34 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26.3-alpine`

```console
$ docker pull telegraf@sha256:6324054ecb1955be213e63944c66a84a8fd98972aa93f95d116dc8c4524e5c2a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.26.3-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:78f7670b9bcd3a4aad80c6ebbee49cf7335f6a5d2d859c953bfa64f8006f38e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.4 MB (56442923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84c98ff0b99b251029050997eaa7c7f4781b917a79b8bed512a729e69982f7c2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 20:30:41 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:04:25 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 09 Aug 2023 04:04:40 GMT
ENV TELEGRAF_VERSION=1.26.3
# Wed, 09 Aug 2023 04:04:52 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 09 Aug 2023 04:04:52 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 09 Aug 2023 04:04:52 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 09 Aug 2023 04:04:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:04:52 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bdca2725167af68b5a2e88c072759b23a3bf0e32c8526c7e9b89f616db5a88d`  
		Last Modified: Mon, 07 Aug 2023 20:31:39 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81f19a7d917a9734911b177e41983aa98776e1138b57753de6adba42dd022ba`  
		Last Modified: Wed, 09 Aug 2023 04:05:25 GMT  
		Size: 2.7 MB (2671751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ffe32ffc35ea9bbf469c7313d2e28eb55dce4def6d7921b4a8ed64d5065827`  
		Last Modified: Wed, 09 Aug 2023 04:05:49 GMT  
		Size: 50.4 MB (50391957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adf8ae69b2b52e8bf419120908053a720d3c85e1cd6eee473ce91f75e98b516a`  
		Last Modified: Wed, 09 Aug 2023 04:05:41 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26.3-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:e663774ce831002c89534e1f287e55d3bd316713b618e67701db26fbe5d8028d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51774942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8375fdb742f718828f27c8a87bcacfe958d4efe3802049d8e0f2db47b8b63653`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 00:46:08 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:25:36 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 09 Aug 2023 04:25:36 GMT
ENV TELEGRAF_VERSION=1.26.3
# Wed, 09 Aug 2023 04:25:43 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 09 Aug 2023 04:25:44 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 09 Aug 2023 04:25:44 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 09 Aug 2023 04:25:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:25:44 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd1799839c258f2f362340c258c49aa080e354fd0e137266f54d413ef004a1b`  
		Last Modified: Wed, 09 Aug 2023 00:46:37 GMT  
		Size: 283.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47f27f99383dfe7b1872c5a815d6081f46d86eeaa05a1cb0fef13827b0fe766`  
		Last Modified: Wed, 09 Aug 2023 04:26:17 GMT  
		Size: 2.7 MB (2703763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014a294016445a25dbb6ffc116ee7cabe334d80ec4a227196a4109180dbe204b`  
		Last Modified: Wed, 09 Aug 2023 04:26:22 GMT  
		Size: 45.8 MB (45812279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8399f752cf89525b188eb16e83df90ab39e25524c9308c289d2f748445fca4`  
		Last Modified: Wed, 09 Aug 2023 04:26:16 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.27`

```console
$ docker pull telegraf@sha256:9eef55aa5c230c6111d7c061be7621a9e6e64e6a3ee12c5cfa8d72ff8e49b3a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.27` - linux; amd64

```console
$ docker pull telegraf@sha256:5f7c7fca0cba5cb57f233a9af314807852148195a0bb0d1d2a3beb9351860b04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.9 MB (147932370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb489fba9df6e62aaf219962c0a231332d90fd7a2339e7077c28a25552b0aa45`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:30 GMT
ADD file:3a6d159d80cb8abfacda5873c243a6ae635ff603708febc4df51f8eec26d3de7 in / 
# Wed, 16 Aug 2023 00:59:31 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:57:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 00:55:22 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 00:55:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Aug 2023 00:55:24 GMT
ENV TELEGRAF_VERSION=1.27.3
# Thu, 17 Aug 2023 00:55:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 17 Aug 2023 00:55:28 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 17 Aug 2023 00:55:28 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 17 Aug 2023 00:55:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Aug 2023 00:55:28 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:de4cac68b6165c40cf6f8b30417948c31be03a968e233e55ee40221553a5e570`  
		Last Modified: Wed, 16 Aug 2023 01:04:06 GMT  
		Size: 49.6 MB (49557399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31b0195ec5f04dfc78eca9d73b5d223fc36a29f54ee888bc4e0615b5839e692`  
		Last Modified: Wed, 16 Aug 2023 07:12:39 GMT  
		Size: 24.0 MB (24030511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6552e3aa56958396ea9000e055520509fe3d67d0f68930c9ac3635a01b371a`  
		Last Modified: Thu, 17 Aug 2023 00:56:24 GMT  
		Size: 19.1 MB (19143607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589e35cc4c9d22bf62f5d4eab0732ef157c4086bb8869113f89a0a81f4052c5d`  
		Last Modified: Thu, 17 Aug 2023 00:56:21 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf9f42f86d7ae3d3ad8c3cfb351697fa9120c7e129758c75619b12a6d8d4150`  
		Last Modified: Thu, 17 Aug 2023 00:56:29 GMT  
		Size: 55.2 MB (55198704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c96fac54c44e814fad9c6320ccae3dbedff7ab40d112dc6a25ad46e0c606cde`  
		Last Modified: Thu, 17 Aug 2023 00:56:21 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:11161e8d3ba4ec2ec3e84c9b4f467817b4de2aa736e811d5de71954c8284cfaf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.5 MB (136542782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41f4e91ebe11cc5a5d61fc52e54fe58933a5a966c8b71903d77c5a0ed527834d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 16 Aug 2023 00:16:59 GMT
ADD file:03964ab92340a6f07fac7e332ca5f5401b3a35aa1e4a5c0b2484a71ff345bc29 in / 
# Wed, 16 Aug 2023 00:16:59 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 21:46:07 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 21:46:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Aug 2023 21:46:09 GMT
ENV TELEGRAF_VERSION=1.27.3
# Wed, 16 Aug 2023 21:46:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 16 Aug 2023 21:46:16 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 16 Aug 2023 21:46:16 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 16 Aug 2023 21:46:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Aug 2023 21:46:16 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:22c91d9cbb3cbc0e4a05c1bfc86da0b5a439ded4f68eb2fbc055ba6b85ca1d90`  
		Last Modified: Wed, 16 Aug 2023 00:21:04 GMT  
		Size: 45.2 MB (45232937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24238a7fc18d7c6089f4f19e3e3d866f42674716043768c48cf6cabb7c8855b0`  
		Last Modified: Wed, 16 Aug 2023 05:47:31 GMT  
		Size: 21.9 MB (21936925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4136b5069a32b3e75c4401bafaaebbd14020c9c796608200fbb58b7f8e501fad`  
		Last Modified: Wed, 16 Aug 2023 21:47:05 GMT  
		Size: 18.0 MB (17989197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3b4492a7ea907433ba641a18fbfee37063deaa9b261a9256cfad10885e0ff2`  
		Last Modified: Wed, 16 Aug 2023 21:47:01 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb731d500e6ac848e2a1c77ccff128ea3d600ac93c0873ab57c5cb74207adf6c`  
		Last Modified: Wed, 16 Aug 2023 21:47:10 GMT  
		Size: 51.4 MB (51381575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eacffefe40b87b80d9919717a65643aa681470667079aaf67e95c5db58cebf33`  
		Last Modified: Wed, 16 Aug 2023 21:47:01 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:bb8fe3ebf848636359b3788172b7a3b1370bf8ac7812c416ae9601a31599c391
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.1 MB (142083353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b0c63bd03757347602fffd84065b9bb5b18902d631a1dd672a147cfeab0cb69`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:49 GMT
ADD file:ca43018e3d97d44b49e60fe002bb20834a74cc1163d7e95ad50d549f072de158 in / 
# Tue, 15 Aug 2023 23:39:49 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:21:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 23:00:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 23:00:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Aug 2023 23:00:01 GMT
ENV TELEGRAF_VERSION=1.27.3
# Wed, 16 Aug 2023 23:00:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 16 Aug 2023 23:00:06 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 16 Aug 2023 23:00:06 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 16 Aug 2023 23:00:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Aug 2023 23:00:06 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a014e5e7d08c37cf1703b97e701ccdc850e4a18d0ee679f03aa875dcd520aa85`  
		Last Modified: Tue, 15 Aug 2023 23:42:59 GMT  
		Size: 49.6 MB (49591310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715cea74ecbb15cb82efef1e77dd60c31d90b01d1286d6f39b4562afaebe75f3`  
		Last Modified: Wed, 16 Aug 2023 01:38:30 GMT  
		Size: 23.6 MB (23570046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58121fe4abd88f975020d3205911dfdcbf27a7bd72628f083186bfc6fbb9cf2`  
		Last Modified: Wed, 16 Aug 2023 23:00:51 GMT  
		Size: 19.1 MB (19077113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6997a7c465673ef3826712aff5a6ad2532f97774caea70aed6ea6f23e22575fb`  
		Last Modified: Wed, 16 Aug 2023 23:00:48 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b854c4748f18f843da8a7f9a7d932a5ed445cf1c2b97bf8159228aa35cf5816`  
		Last Modified: Wed, 16 Aug 2023 23:00:54 GMT  
		Size: 49.8 MB (49842741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc00fa1181a674ddb859e618bf3414abf6a32bf60ab4e854e0f206dd3c40bf9`  
		Last Modified: Wed, 16 Aug 2023 23:00:48 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.27-alpine`

```console
$ docker pull telegraf@sha256:90a47ae732d43805f1c425bf73304fbdf47efb51cd7af0fb49e79c98195a504a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.27-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:399b37278a5cd8ec1f2524b9cd0e775c27a87e779177de66917695a4e9ab93aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.1 MB (61085260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e85a38d285b30401f09c663ce4a2a36ba95adf896e1d54c028abca5e985efcfd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:05:00 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:05:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 09 Aug 2023 04:05:02 GMT
ENV TELEGRAF_VERSION=1.27.3
# Wed, 09 Aug 2023 04:05:08 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 09 Aug 2023 04:05:08 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 09 Aug 2023 04:05:08 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 09 Aug 2023 04:05:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:05:09 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039529048aa7cd46b974231fd34d48f954eb067994d5f425569af914e7de0ef6`  
		Last Modified: Wed, 09 Aug 2023 04:05:58 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96767576f65551b43cd2f308297af5090afedffb7eb547e395c8c2e02d848397`  
		Last Modified: Wed, 09 Aug 2023 04:05:59 GMT  
		Size: 2.6 MB (2643772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa041e5ec23180dc1cf466bd7f77b9cf1da086a20e0b81c192dfbf2f8a9a23c`  
		Last Modified: Wed, 09 Aug 2023 04:06:07 GMT  
		Size: 55.0 MB (55039266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2de8e60566a11fbd062faaf9f3c9e2cf4d5270268747f644f3eea642dee69b`  
		Last Modified: Wed, 09 Aug 2023 04:05:58 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:f8d7ecac237aa2eef3ac600f5fde92a118fd6ecd6ccd1a79e2b60cb8a27ac3ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55672923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7866c614bf015ce71a52bf5ae87ab7bddf0c470eb6f43fbb05e2d2a4df0d96ec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:25:48 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:25:50 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 09 Aug 2023 04:25:50 GMT
ENV TELEGRAF_VERSION=1.27.3
# Wed, 09 Aug 2023 04:25:57 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 09 Aug 2023 04:25:58 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 09 Aug 2023 04:25:58 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 09 Aug 2023 04:25:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:25:58 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d4096012e5a9408aedb4891d96f73d6678d25354afc929941aa2338446c730`  
		Last Modified: Wed, 09 Aug 2023 04:26:31 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a312960d045953e25342cafbc53ced993bfc32dfe9e0cebfaf28769e1b2f481`  
		Last Modified: Wed, 09 Aug 2023 04:26:32 GMT  
		Size: 2.7 MB (2671154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3963f4280f5eb1058da408938509b98d3db7256fde0f91c9457be1c41d175cee`  
		Last Modified: Wed, 09 Aug 2023 04:26:37 GMT  
		Size: 49.7 MB (49670393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7822a5fb6b5cf3547f05c92af6e1ef19b26fb4010422ad511c2a8f0ac47acd74`  
		Last Modified: Wed, 09 Aug 2023 04:26:31 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.27.4`

```console
$ docker pull telegraf@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `telegraf:1.27.4-alpine`

```console
$ docker pull telegraf@sha256:eb37f58646a901dc7727cf448cae36daaefaba79de33b5058dab79aa4c04aefb
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 0

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:90a47ae732d43805f1c425bf73304fbdf47efb51cd7af0fb49e79c98195a504a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:399b37278a5cd8ec1f2524b9cd0e775c27a87e779177de66917695a4e9ab93aa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.1 MB (61085260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e85a38d285b30401f09c663ce4a2a36ba95adf896e1d54c028abca5e985efcfd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:05:00 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:05:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 09 Aug 2023 04:05:02 GMT
ENV TELEGRAF_VERSION=1.27.3
# Wed, 09 Aug 2023 04:05:08 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 09 Aug 2023 04:05:08 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 09 Aug 2023 04:05:08 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 09 Aug 2023 04:05:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:05:09 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:039529048aa7cd46b974231fd34d48f954eb067994d5f425569af914e7de0ef6`  
		Last Modified: Wed, 09 Aug 2023 04:05:58 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96767576f65551b43cd2f308297af5090afedffb7eb547e395c8c2e02d848397`  
		Last Modified: Wed, 09 Aug 2023 04:05:59 GMT  
		Size: 2.6 MB (2643772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa041e5ec23180dc1cf466bd7f77b9cf1da086a20e0b81c192dfbf2f8a9a23c`  
		Last Modified: Wed, 09 Aug 2023 04:06:07 GMT  
		Size: 55.0 MB (55039266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef2de8e60566a11fbd062faaf9f3c9e2cf4d5270268747f644f3eea642dee69b`  
		Last Modified: Wed, 09 Aug 2023 04:05:58 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:f8d7ecac237aa2eef3ac600f5fde92a118fd6ecd6ccd1a79e2b60cb8a27ac3ca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.7 MB (55672923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7866c614bf015ce71a52bf5ae87ab7bddf0c470eb6f43fbb05e2d2a4df0d96ec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:19 GMT
ADD file:b2e7eaa7e41f08853dbe08d84439a7f9fd32fc58c3aa1e298f3f60343b2b683a in / 
# Mon, 07 Aug 2023 19:39:19 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:25:48 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 09 Aug 2023 04:25:50 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 09 Aug 2023 04:25:50 GMT
ENV TELEGRAF_VERSION=1.27.3
# Wed, 09 Aug 2023 04:25:57 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 09 Aug 2023 04:25:58 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 09 Aug 2023 04:25:58 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 09 Aug 2023 04:25:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 09 Aug 2023 04:25:58 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:9fda8d8052c61740409c4bea888859c141fd8cc3f58ac61943144ff6d1681b2d`  
		Last Modified: Mon, 07 Aug 2023 19:39:45 GMT  
		Size: 3.3 MB (3330767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d4096012e5a9408aedb4891d96f73d6678d25354afc929941aa2338446c730`  
		Last Modified: Wed, 09 Aug 2023 04:26:31 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a312960d045953e25342cafbc53ced993bfc32dfe9e0cebfaf28769e1b2f481`  
		Last Modified: Wed, 09 Aug 2023 04:26:32 GMT  
		Size: 2.7 MB (2671154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3963f4280f5eb1058da408938509b98d3db7256fde0f91c9457be1c41d175cee`  
		Last Modified: Wed, 09 Aug 2023 04:26:37 GMT  
		Size: 49.7 MB (49670393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7822a5fb6b5cf3547f05c92af6e1ef19b26fb4010422ad511c2a8f0ac47acd74`  
		Last Modified: Wed, 09 Aug 2023 04:26:31 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:9eef55aa5c230c6111d7c061be7621a9e6e64e6a3ee12c5cfa8d72ff8e49b3a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:5f7c7fca0cba5cb57f233a9af314807852148195a0bb0d1d2a3beb9351860b04
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.9 MB (147932370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb489fba9df6e62aaf219962c0a231332d90fd7a2339e7077c28a25552b0aa45`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 16 Aug 2023 00:59:30 GMT
ADD file:3a6d159d80cb8abfacda5873c243a6ae635ff603708febc4df51f8eec26d3de7 in / 
# Wed, 16 Aug 2023 00:59:31 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 06:57:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 00:55:22 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 17 Aug 2023 00:55:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 17 Aug 2023 00:55:24 GMT
ENV TELEGRAF_VERSION=1.27.3
# Thu, 17 Aug 2023 00:55:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 17 Aug 2023 00:55:28 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 17 Aug 2023 00:55:28 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 17 Aug 2023 00:55:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 17 Aug 2023 00:55:28 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:de4cac68b6165c40cf6f8b30417948c31be03a968e233e55ee40221553a5e570`  
		Last Modified: Wed, 16 Aug 2023 01:04:06 GMT  
		Size: 49.6 MB (49557399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31b0195ec5f04dfc78eca9d73b5d223fc36a29f54ee888bc4e0615b5839e692`  
		Last Modified: Wed, 16 Aug 2023 07:12:39 GMT  
		Size: 24.0 MB (24030511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6552e3aa56958396ea9000e055520509fe3d67d0f68930c9ac3635a01b371a`  
		Last Modified: Thu, 17 Aug 2023 00:56:24 GMT  
		Size: 19.1 MB (19143607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:589e35cc4c9d22bf62f5d4eab0732ef157c4086bb8869113f89a0a81f4052c5d`  
		Last Modified: Thu, 17 Aug 2023 00:56:21 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cf9f42f86d7ae3d3ad8c3cfb351697fa9120c7e129758c75619b12a6d8d4150`  
		Last Modified: Thu, 17 Aug 2023 00:56:29 GMT  
		Size: 55.2 MB (55198704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c96fac54c44e814fad9c6320ccae3dbedff7ab40d112dc6a25ad46e0c606cde`  
		Last Modified: Thu, 17 Aug 2023 00:56:21 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:11161e8d3ba4ec2ec3e84c9b4f467817b4de2aa736e811d5de71954c8284cfaf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.5 MB (136542782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41f4e91ebe11cc5a5d61fc52e54fe58933a5a966c8b71903d77c5a0ed527834d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 16 Aug 2023 00:16:59 GMT
ADD file:03964ab92340a6f07fac7e332ca5f5401b3a35aa1e4a5c0b2484a71ff345bc29 in / 
# Wed, 16 Aug 2023 00:16:59 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 21:46:07 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 21:46:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Aug 2023 21:46:09 GMT
ENV TELEGRAF_VERSION=1.27.3
# Wed, 16 Aug 2023 21:46:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 16 Aug 2023 21:46:16 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 16 Aug 2023 21:46:16 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 16 Aug 2023 21:46:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Aug 2023 21:46:16 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:22c91d9cbb3cbc0e4a05c1bfc86da0b5a439ded4f68eb2fbc055ba6b85ca1d90`  
		Last Modified: Wed, 16 Aug 2023 00:21:04 GMT  
		Size: 45.2 MB (45232937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24238a7fc18d7c6089f4f19e3e3d866f42674716043768c48cf6cabb7c8855b0`  
		Last Modified: Wed, 16 Aug 2023 05:47:31 GMT  
		Size: 21.9 MB (21936925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4136b5069a32b3e75c4401bafaaebbd14020c9c796608200fbb58b7f8e501fad`  
		Last Modified: Wed, 16 Aug 2023 21:47:05 GMT  
		Size: 18.0 MB (17989197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3b4492a7ea907433ba641a18fbfee37063deaa9b261a9256cfad10885e0ff2`  
		Last Modified: Wed, 16 Aug 2023 21:47:01 GMT  
		Size: 1.8 KB (1803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb731d500e6ac848e2a1c77ccff128ea3d600ac93c0873ab57c5cb74207adf6c`  
		Last Modified: Wed, 16 Aug 2023 21:47:10 GMT  
		Size: 51.4 MB (51381575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eacffefe40b87b80d9919717a65643aa681470667079aaf67e95c5db58cebf33`  
		Last Modified: Wed, 16 Aug 2023 21:47:01 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:bb8fe3ebf848636359b3788172b7a3b1370bf8ac7812c416ae9601a31599c391
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.1 MB (142083353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b0c63bd03757347602fffd84065b9bb5b18902d631a1dd672a147cfeab0cb69`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:49 GMT
ADD file:ca43018e3d97d44b49e60fe002bb20834a74cc1163d7e95ad50d549f072de158 in / 
# Tue, 15 Aug 2023 23:39:49 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:21:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 23:00:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 23:00:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 16 Aug 2023 23:00:01 GMT
ENV TELEGRAF_VERSION=1.27.3
# Wed, 16 Aug 2023 23:00:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 16 Aug 2023 23:00:06 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 16 Aug 2023 23:00:06 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 16 Aug 2023 23:00:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Aug 2023 23:00:06 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a014e5e7d08c37cf1703b97e701ccdc850e4a18d0ee679f03aa875dcd520aa85`  
		Last Modified: Tue, 15 Aug 2023 23:42:59 GMT  
		Size: 49.6 MB (49591310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715cea74ecbb15cb82efef1e77dd60c31d90b01d1286d6f39b4562afaebe75f3`  
		Last Modified: Wed, 16 Aug 2023 01:38:30 GMT  
		Size: 23.6 MB (23570046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58121fe4abd88f975020d3205911dfdcbf27a7bd72628f083186bfc6fbb9cf2`  
		Last Modified: Wed, 16 Aug 2023 23:00:51 GMT  
		Size: 19.1 MB (19077113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6997a7c465673ef3826712aff5a6ad2532f97774caea70aed6ea6f23e22575fb`  
		Last Modified: Wed, 16 Aug 2023 23:00:48 GMT  
		Size: 1.8 KB (1801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b854c4748f18f843da8a7f9a7d932a5ed445cf1c2b97bf8159228aa35cf5816`  
		Last Modified: Wed, 16 Aug 2023 23:00:54 GMT  
		Size: 49.8 MB (49842741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc00fa1181a674ddb859e618bf3414abf6a32bf60ab4e854e0f206dd3c40bf9`  
		Last Modified: Wed, 16 Aug 2023 23:00:48 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
