<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `telegraf`

-	[`telegraf:1.23`](#telegraf123)
-	[`telegraf:1.23-alpine`](#telegraf123-alpine)
-	[`telegraf:1.23.4`](#telegraf1234)
-	[`telegraf:1.23.4-alpine`](#telegraf1234-alpine)
-	[`telegraf:1.24`](#telegraf124)
-	[`telegraf:1.24-alpine`](#telegraf124-alpine)
-	[`telegraf:1.24.4`](#telegraf1244)
-	[`telegraf:1.24.4-alpine`](#telegraf1244-alpine)
-	[`telegraf:1.25`](#telegraf125)
-	[`telegraf:1.25-alpine`](#telegraf125-alpine)
-	[`telegraf:1.25.1`](#telegraf1251)
-	[`telegraf:1.25.1-alpine`](#telegraf1251-alpine)
-	[`telegraf:alpine`](#telegrafalpine)
-	[`telegraf:latest`](#telegraflatest)

## `telegraf:1.23`

```console
$ docker pull telegraf@sha256:8c12f1ed9935a988ef057895e12042b93ec6c3b615a350493291b959dde5e11b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.23` - linux; amd64

```console
$ docker pull telegraf@sha256:0166e317438e0350c6d9ff5297b2c2dfd4d3c50ed145f12d7aef8af20ec4f780
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131678820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82c7cb34db41d4f6979d8ebf942a15ff01fb3afc9b0f1d0c5fe574d277d724a9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:26 GMT
ADD file:cc6a56676703ec7ab5db8f2f7bc18a3169c0816d38703845b6b77ae5342ab41c in / 
# Sat, 04 Feb 2023 06:51:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:22:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:22:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 05 Feb 2023 00:17:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 00:17:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 05 Feb 2023 00:17:13 GMT
ENV TELEGRAF_VERSION=1.23.4
# Sun, 05 Feb 2023 00:17:18 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sun, 05 Feb 2023 00:17:19 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sun, 05 Feb 2023 00:17:19 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sun, 05 Feb 2023 00:17:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 05 Feb 2023 00:17:19 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:699c8a97647f5789e5850bcf1a3d5afe9730edb654e1ae0714d5bd198a67a3ed`  
		Last Modified: Sat, 04 Feb 2023 06:55:53 GMT  
		Size: 55.0 MB (55025312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cd158b89fde67a8a4c428a844985f930eba450ec3fde1c9ef5df3884128c62`  
		Last Modified: Sat, 04 Feb 2023 07:29:25 GMT  
		Size: 5.2 MB (5165476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226e961cfaa2d1d171e429e9db314feec6201f5cba1487b20e7aee311e4a54f`  
		Last Modified: Sat, 04 Feb 2023 07:29:25 GMT  
		Size: 10.9 MB (10876697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57437773f0bea58cfa95e8754b53e61f4b2a0a91db902a4b6889886bbd32379f`  
		Last Modified: Sun, 05 Feb 2023 00:18:10 GMT  
		Size: 18.8 MB (18759957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578db7ef68ed573b90f714e49ff85d02b23dc49a904a5a56d51cbff9a5466897`  
		Last Modified: Sun, 05 Feb 2023 00:18:07 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2121a419d8fe05d0b5990d768bfadb72254c7b5e39bdaa1fd7190df6fa92b1`  
		Last Modified: Sun, 05 Feb 2023 00:18:14 GMT  
		Size: 41.8 MB (41849227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec23b9e1613a3562edb0fdc96b573f019f646a72061050f1154d4fbb0b1fe03`  
		Last Modified: Sun, 05 Feb 2023 00:18:07 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:ace0f9a7bdb342e5fb3b42a23d3a9450bdc8257bc1f4c7dd47ac1a5fea09557d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121912862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:349f4063ce20243c12a98d03ebcb7ff2ee4c415eaaaa6459845788870113894e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:19 GMT
ADD file:239b5255d05e0742f381f82fb7cd586fcc6d9a427263238a2be3372c494ae933 in / 
# Sat, 04 Feb 2023 09:59:20 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:49:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:49:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 05 Feb 2023 05:46:36 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 05:46:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 05 Feb 2023 05:46:38 GMT
ENV TELEGRAF_VERSION=1.23.4
# Sun, 05 Feb 2023 05:46:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sun, 05 Feb 2023 05:46:44 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sun, 05 Feb 2023 05:46:44 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sun, 05 Feb 2023 05:46:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 05 Feb 2023 05:46:45 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:7a21a86b3957d8c99250334cfb78c55af4f8c9277f2f1d4abd53d0362f96323d`  
		Last Modified: Sat, 04 Feb 2023 10:05:53 GMT  
		Size: 50.2 MB (50190828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aacc3c746ca1bd99005f184b00ee418e015c2090c72bda638766d9fb93d3f065`  
		Last Modified: Sat, 04 Feb 2023 10:59:08 GMT  
		Size: 4.9 MB (4933374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b393b343e4fb3b92027c4741418a04d6475259ee243fbf036c1be41df98212`  
		Last Modified: Sat, 04 Feb 2023 10:59:09 GMT  
		Size: 10.2 MB (10217742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46cdeffc1bc9c2d2ce2391093aa478f8a199e3acd00a74991621f53f0c78cb0`  
		Last Modified: Sun, 05 Feb 2023 05:47:43 GMT  
		Size: 17.5 MB (17462246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1302093fdb79f487f8a36fe43c509b03e014f5d1dd15a8bb06b8499d2bd57616`  
		Last Modified: Sun, 05 Feb 2023 05:47:39 GMT  
		Size: 1.8 KB (1780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16633da1d2ddc144e5ca32a054d47a77e740d1b90076ffb8d8a10f426b6805cb`  
		Last Modified: Sun, 05 Feb 2023 05:47:46 GMT  
		Size: 39.1 MB (39106550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b74b12a93a2712c6bc4cb32003a6a500d9c522d664a99c1974ab4cf6a50985`  
		Last Modified: Sun, 05 Feb 2023 05:47:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:803ce566e208b5f8124c5d9110231d74e1e36813f23c72bab336d0dcae25fad5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126360871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ada1da98a288fa93eb3b3c3532d9f71b94386aa5da0c3204aba83364c9711d87`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:08:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:08:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 21:12:59 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 21:13:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 09 Feb 2023 21:13:01 GMT
ENV TELEGRAF_VERSION=1.23.4
# Thu, 09 Feb 2023 21:13:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 09 Feb 2023 21:13:06 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 09 Feb 2023 21:13:06 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 09 Feb 2023 21:13:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 09 Feb 2023 21:13:06 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae98695cf4875b92116a031bcf51736705c39b105be5f240a143935d8370f6`  
		Last Modified: Thu, 09 Feb 2023 09:14:20 GMT  
		Size: 5.2 MB (5152064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a74e69230a5d5ee55fb6baca6fb52404417efd177a2cb03c418d2d0cf599b5`  
		Last Modified: Thu, 09 Feb 2023 09:14:21 GMT  
		Size: 10.9 MB (10873498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a8c92acaa189d96003ac9c932821ad706b110685d6134804937c672a32cfce`  
		Last Modified: Thu, 09 Feb 2023 21:13:38 GMT  
		Size: 18.6 MB (18598477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8453344745624d949ed6cc91b95bf6b64abdcf79c0b29df0cee561116e2780fc`  
		Last Modified: Thu, 09 Feb 2023 21:13:35 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d473f1eec5c3dcb1d5c7294b693bbec569739a50d80506187158d7cf1aab05cd`  
		Last Modified: Thu, 09 Feb 2023 21:13:40 GMT  
		Size: 38.0 MB (38031312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17533e605e0d05eacbff5dc53b26578293af1bf87f0e63acf06d6488bd756ad4`  
		Last Modified: Thu, 09 Feb 2023 21:13:35 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.23-alpine`

```console
$ docker pull telegraf@sha256:1926cd26e2513a7accae2c8f6d2f529913d8014e9abd0179c7e5bf6e90ef047c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.23-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:9b0df9667fcceac0af01b504652981fb545ea69c830e4401a23b0bb0c74e2405
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47790823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f32baa5e4356d4cb3dbd13b6f57a6c46e41e16fbcd09427afb97a2611c786e5f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:32:05 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 12 Nov 2022 10:02:29 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Sat, 12 Nov 2022 10:02:41 GMT
ENV TELEGRAF_VERSION=1.23.4
# Wed, 01 Feb 2023 21:42:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 01 Feb 2023 21:42:23 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 01 Feb 2023 21:42:23 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 01 Feb 2023 21:42:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 21:42:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec8c4909872f004bb7fe69291336b9a1be138c76e18c8706b787cce0ddf850c`  
		Last Modified: Sat, 12 Nov 2022 08:32:35 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb65cee31d4b1da1248e34183af68dd614828735af79e4ec9c1967a3cfe0718`  
		Last Modified: Sat, 12 Nov 2022 10:03:26 GMT  
		Size: 3.3 MB (3298059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89c8bf1101b7f5fe6e4c1f292a4f6f423ad10b4091d0027b11b8d855ecbe889`  
		Last Modified: Wed, 01 Feb 2023 21:43:41 GMT  
		Size: 41.7 MB (41685883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1b5ca8e7c11770726e4f893d584288acd1846c0e379f2e46a4cb42d0d473df`  
		Last Modified: Wed, 01 Feb 2023 21:43:34 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.23.4`

```console
$ docker pull telegraf@sha256:8c12f1ed9935a988ef057895e12042b93ec6c3b615a350493291b959dde5e11b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.23.4` - linux; amd64

```console
$ docker pull telegraf@sha256:0166e317438e0350c6d9ff5297b2c2dfd4d3c50ed145f12d7aef8af20ec4f780
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131678820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82c7cb34db41d4f6979d8ebf942a15ff01fb3afc9b0f1d0c5fe574d277d724a9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:26 GMT
ADD file:cc6a56676703ec7ab5db8f2f7bc18a3169c0816d38703845b6b77ae5342ab41c in / 
# Sat, 04 Feb 2023 06:51:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:22:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:22:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 05 Feb 2023 00:17:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 00:17:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 05 Feb 2023 00:17:13 GMT
ENV TELEGRAF_VERSION=1.23.4
# Sun, 05 Feb 2023 00:17:18 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sun, 05 Feb 2023 00:17:19 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sun, 05 Feb 2023 00:17:19 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sun, 05 Feb 2023 00:17:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 05 Feb 2023 00:17:19 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:699c8a97647f5789e5850bcf1a3d5afe9730edb654e1ae0714d5bd198a67a3ed`  
		Last Modified: Sat, 04 Feb 2023 06:55:53 GMT  
		Size: 55.0 MB (55025312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cd158b89fde67a8a4c428a844985f930eba450ec3fde1c9ef5df3884128c62`  
		Last Modified: Sat, 04 Feb 2023 07:29:25 GMT  
		Size: 5.2 MB (5165476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226e961cfaa2d1d171e429e9db314feec6201f5cba1487b20e7aee311e4a54f`  
		Last Modified: Sat, 04 Feb 2023 07:29:25 GMT  
		Size: 10.9 MB (10876697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57437773f0bea58cfa95e8754b53e61f4b2a0a91db902a4b6889886bbd32379f`  
		Last Modified: Sun, 05 Feb 2023 00:18:10 GMT  
		Size: 18.8 MB (18759957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578db7ef68ed573b90f714e49ff85d02b23dc49a904a5a56d51cbff9a5466897`  
		Last Modified: Sun, 05 Feb 2023 00:18:07 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2121a419d8fe05d0b5990d768bfadb72254c7b5e39bdaa1fd7190df6fa92b1`  
		Last Modified: Sun, 05 Feb 2023 00:18:14 GMT  
		Size: 41.8 MB (41849227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec23b9e1613a3562edb0fdc96b573f019f646a72061050f1154d4fbb0b1fe03`  
		Last Modified: Sun, 05 Feb 2023 00:18:07 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23.4` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:ace0f9a7bdb342e5fb3b42a23d3a9450bdc8257bc1f4c7dd47ac1a5fea09557d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.9 MB (121912862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:349f4063ce20243c12a98d03ebcb7ff2ee4c415eaaaa6459845788870113894e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:19 GMT
ADD file:239b5255d05e0742f381f82fb7cd586fcc6d9a427263238a2be3372c494ae933 in / 
# Sat, 04 Feb 2023 09:59:20 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:49:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:49:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 05 Feb 2023 05:46:36 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 05:46:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 05 Feb 2023 05:46:38 GMT
ENV TELEGRAF_VERSION=1.23.4
# Sun, 05 Feb 2023 05:46:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sun, 05 Feb 2023 05:46:44 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sun, 05 Feb 2023 05:46:44 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sun, 05 Feb 2023 05:46:44 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 05 Feb 2023 05:46:45 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:7a21a86b3957d8c99250334cfb78c55af4f8c9277f2f1d4abd53d0362f96323d`  
		Last Modified: Sat, 04 Feb 2023 10:05:53 GMT  
		Size: 50.2 MB (50190828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aacc3c746ca1bd99005f184b00ee418e015c2090c72bda638766d9fb93d3f065`  
		Last Modified: Sat, 04 Feb 2023 10:59:08 GMT  
		Size: 4.9 MB (4933374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b393b343e4fb3b92027c4741418a04d6475259ee243fbf036c1be41df98212`  
		Last Modified: Sat, 04 Feb 2023 10:59:09 GMT  
		Size: 10.2 MB (10217742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46cdeffc1bc9c2d2ce2391093aa478f8a199e3acd00a74991621f53f0c78cb0`  
		Last Modified: Sun, 05 Feb 2023 05:47:43 GMT  
		Size: 17.5 MB (17462246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1302093fdb79f487f8a36fe43c509b03e014f5d1dd15a8bb06b8499d2bd57616`  
		Last Modified: Sun, 05 Feb 2023 05:47:39 GMT  
		Size: 1.8 KB (1780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16633da1d2ddc144e5ca32a054d47a77e740d1b90076ffb8d8a10f426b6805cb`  
		Last Modified: Sun, 05 Feb 2023 05:47:46 GMT  
		Size: 39.1 MB (39106550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b74b12a93a2712c6bc4cb32003a6a500d9c522d664a99c1974ab4cf6a50985`  
		Last Modified: Sun, 05 Feb 2023 05:47:39 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.23.4` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:803ce566e208b5f8124c5d9110231d74e1e36813f23c72bab336d0dcae25fad5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126360871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ada1da98a288fa93eb3b3c3532d9f71b94386aa5da0c3204aba83364c9711d87`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:08:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:08:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 21:12:59 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 21:13:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 09 Feb 2023 21:13:01 GMT
ENV TELEGRAF_VERSION=1.23.4
# Thu, 09 Feb 2023 21:13:05 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 09 Feb 2023 21:13:06 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 09 Feb 2023 21:13:06 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 09 Feb 2023 21:13:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 09 Feb 2023 21:13:06 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae98695cf4875b92116a031bcf51736705c39b105be5f240a143935d8370f6`  
		Last Modified: Thu, 09 Feb 2023 09:14:20 GMT  
		Size: 5.2 MB (5152064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a74e69230a5d5ee55fb6baca6fb52404417efd177a2cb03c418d2d0cf599b5`  
		Last Modified: Thu, 09 Feb 2023 09:14:21 GMT  
		Size: 10.9 MB (10873498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a8c92acaa189d96003ac9c932821ad706b110685d6134804937c672a32cfce`  
		Last Modified: Thu, 09 Feb 2023 21:13:38 GMT  
		Size: 18.6 MB (18598477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8453344745624d949ed6cc91b95bf6b64abdcf79c0b29df0cee561116e2780fc`  
		Last Modified: Thu, 09 Feb 2023 21:13:35 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d473f1eec5c3dcb1d5c7294b693bbec569739a50d80506187158d7cf1aab05cd`  
		Last Modified: Thu, 09 Feb 2023 21:13:40 GMT  
		Size: 38.0 MB (38031312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17533e605e0d05eacbff5dc53b26578293af1bf87f0e63acf06d6488bd756ad4`  
		Last Modified: Thu, 09 Feb 2023 21:13:35 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.23.4-alpine`

```console
$ docker pull telegraf@sha256:1926cd26e2513a7accae2c8f6d2f529913d8014e9abd0179c7e5bf6e90ef047c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.23.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:9b0df9667fcceac0af01b504652981fb545ea69c830e4401a23b0bb0c74e2405
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47790823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f32baa5e4356d4cb3dbd13b6f57a6c46e41e16fbcd09427afb97a2611c786e5f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:32:05 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 12 Nov 2022 10:02:29 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Sat, 12 Nov 2022 10:02:41 GMT
ENV TELEGRAF_VERSION=1.23.4
# Wed, 01 Feb 2023 21:42:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 01 Feb 2023 21:42:23 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 01 Feb 2023 21:42:23 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 01 Feb 2023 21:42:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 21:42:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec8c4909872f004bb7fe69291336b9a1be138c76e18c8706b787cce0ddf850c`  
		Last Modified: Sat, 12 Nov 2022 08:32:35 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb65cee31d4b1da1248e34183af68dd614828735af79e4ec9c1967a3cfe0718`  
		Last Modified: Sat, 12 Nov 2022 10:03:26 GMT  
		Size: 3.3 MB (3298059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89c8bf1101b7f5fe6e4c1f292a4f6f423ad10b4091d0027b11b8d855ecbe889`  
		Last Modified: Wed, 01 Feb 2023 21:43:41 GMT  
		Size: 41.7 MB (41685883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1b5ca8e7c11770726e4f893d584288acd1846c0e379f2e46a4cb42d0d473df`  
		Last Modified: Wed, 01 Feb 2023 21:43:34 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.24`

```console
$ docker pull telegraf@sha256:83a43b1251f4e7ff0083e6e9a4414a5e513b57cb276236cbf6d08cd661b4f825
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.24` - linux; amd64

```console
$ docker pull telegraf@sha256:219891c4a0aec028e69d393f8149d652c054e051723aa8d336ab29926ce263e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134296996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a4580474fe8c87144e34d00df2b5e3afcd0f9c592f00c5cf9ed4c897c7c740b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:26 GMT
ADD file:cc6a56676703ec7ab5db8f2f7bc18a3169c0816d38703845b6b77ae5342ab41c in / 
# Sat, 04 Feb 2023 06:51:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:22:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:22:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 05 Feb 2023 00:17:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 00:17:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 05 Feb 2023 00:17:26 GMT
ENV TELEGRAF_VERSION=1.24.4
# Sun, 05 Feb 2023 00:17:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sun, 05 Feb 2023 00:17:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sun, 05 Feb 2023 00:17:36 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sun, 05 Feb 2023 00:17:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 05 Feb 2023 00:17:36 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:699c8a97647f5789e5850bcf1a3d5afe9730edb654e1ae0714d5bd198a67a3ed`  
		Last Modified: Sat, 04 Feb 2023 06:55:53 GMT  
		Size: 55.0 MB (55025312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cd158b89fde67a8a4c428a844985f930eba450ec3fde1c9ef5df3884128c62`  
		Last Modified: Sat, 04 Feb 2023 07:29:25 GMT  
		Size: 5.2 MB (5165476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226e961cfaa2d1d171e429e9db314feec6201f5cba1487b20e7aee311e4a54f`  
		Last Modified: Sat, 04 Feb 2023 07:29:25 GMT  
		Size: 10.9 MB (10876697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57437773f0bea58cfa95e8754b53e61f4b2a0a91db902a4b6889886bbd32379f`  
		Last Modified: Sun, 05 Feb 2023 00:18:10 GMT  
		Size: 18.8 MB (18759957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578db7ef68ed573b90f714e49ff85d02b23dc49a904a5a56d51cbff9a5466897`  
		Last Modified: Sun, 05 Feb 2023 00:18:07 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8da18d6a92cc4833971872cba24e8a14a30fa846dd0ea80a1b66d422bc5ef76`  
		Last Modified: Sun, 05 Feb 2023 00:18:30 GMT  
		Size: 44.5 MB (44467403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab8e296304a24b6ebbe650fb626a2f434a8a769b7b62d08a650509cb0f8835c`  
		Last Modified: Sun, 05 Feb 2023 00:18:23 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.24` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:5586a64413a0f142389d825d78f9c8c827f1e420032841ef4b75c59cc0930174
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124313376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:588c8f7599ada227ecdbb4bc845749e145cd826184dda24210b59a10247d4def`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:19 GMT
ADD file:239b5255d05e0742f381f82fb7cd586fcc6d9a427263238a2be3372c494ae933 in / 
# Sat, 04 Feb 2023 09:59:20 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:49:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:49:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 05 Feb 2023 05:46:36 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 05:46:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 05 Feb 2023 05:46:51 GMT
ENV TELEGRAF_VERSION=1.24.4
# Sun, 05 Feb 2023 05:46:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sun, 05 Feb 2023 05:46:58 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sun, 05 Feb 2023 05:46:58 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sun, 05 Feb 2023 05:46:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 05 Feb 2023 05:46:58 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:7a21a86b3957d8c99250334cfb78c55af4f8c9277f2f1d4abd53d0362f96323d`  
		Last Modified: Sat, 04 Feb 2023 10:05:53 GMT  
		Size: 50.2 MB (50190828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aacc3c746ca1bd99005f184b00ee418e015c2090c72bda638766d9fb93d3f065`  
		Last Modified: Sat, 04 Feb 2023 10:59:08 GMT  
		Size: 4.9 MB (4933374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b393b343e4fb3b92027c4741418a04d6475259ee243fbf036c1be41df98212`  
		Last Modified: Sat, 04 Feb 2023 10:59:09 GMT  
		Size: 10.2 MB (10217742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46cdeffc1bc9c2d2ce2391093aa478f8a199e3acd00a74991621f53f0c78cb0`  
		Last Modified: Sun, 05 Feb 2023 05:47:43 GMT  
		Size: 17.5 MB (17462246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1302093fdb79f487f8a36fe43c509b03e014f5d1dd15a8bb06b8499d2bd57616`  
		Last Modified: Sun, 05 Feb 2023 05:47:39 GMT  
		Size: 1.8 KB (1780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1033819e1423b511d0d29a8c1fdf787feba297133595dea8c51d27275a7cfc4e`  
		Last Modified: Sun, 05 Feb 2023 05:48:05 GMT  
		Size: 41.5 MB (41507061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94bc6045c8e2194ff2542b1417feca4fe8b6da7b5a6884bddb5a94fcc15656e`  
		Last Modified: Sun, 05 Feb 2023 05:47:57 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.24` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:fc102f828ca9dc2878b61e68bd31609ba1a29e1ccc1500489a03c4d73bdf77bf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128635017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52bc5498388a6a51559b9772559d5ac3e6040317fee182b3d460947e995486e8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:08:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:08:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 21:12:59 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 21:13:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 09 Feb 2023 21:13:09 GMT
ENV TELEGRAF_VERSION=1.24.4
# Thu, 09 Feb 2023 21:13:12 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 09 Feb 2023 21:13:13 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 09 Feb 2023 21:13:13 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 09 Feb 2023 21:13:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 09 Feb 2023 21:13:13 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae98695cf4875b92116a031bcf51736705c39b105be5f240a143935d8370f6`  
		Last Modified: Thu, 09 Feb 2023 09:14:20 GMT  
		Size: 5.2 MB (5152064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a74e69230a5d5ee55fb6baca6fb52404417efd177a2cb03c418d2d0cf599b5`  
		Last Modified: Thu, 09 Feb 2023 09:14:21 GMT  
		Size: 10.9 MB (10873498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a8c92acaa189d96003ac9c932821ad706b110685d6134804937c672a32cfce`  
		Last Modified: Thu, 09 Feb 2023 21:13:38 GMT  
		Size: 18.6 MB (18598477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8453344745624d949ed6cc91b95bf6b64abdcf79c0b29df0cee561116e2780fc`  
		Last Modified: Thu, 09 Feb 2023 21:13:35 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98825686562eec0e4213e16e3734b97e44fa66bc3c69e516e31af1820939f93`  
		Last Modified: Thu, 09 Feb 2023 21:13:54 GMT  
		Size: 40.3 MB (40305460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8318a7b649fffb5e902a0b741a5c54d51ee7b0a6b6715295c031b94293d666b`  
		Last Modified: Thu, 09 Feb 2023 21:13:49 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.24-alpine`

```console
$ docker pull telegraf@sha256:02f7d3ef3ec96fb316c46ef8d9edffda3ef9e1a1674064d692405a3a26466267
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.24-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:2b78bb229fea92cbf8d5de4a73fe57786d4c4bf081728782d2c198c750524564
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50402771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be46e026466d0af78f6c9e4f2b822855db451217c037d63684c71c34e80bcc27`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:32:05 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 12 Nov 2022 10:02:29 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 29 Nov 2022 21:43:37 GMT
ENV TELEGRAF_VERSION=1.24.4
# Wed, 01 Feb 2023 21:42:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 01 Feb 2023 21:42:39 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 01 Feb 2023 21:42:39 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 01 Feb 2023 21:42:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 21:42:40 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec8c4909872f004bb7fe69291336b9a1be138c76e18c8706b787cce0ddf850c`  
		Last Modified: Sat, 12 Nov 2022 08:32:35 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb65cee31d4b1da1248e34183af68dd614828735af79e4ec9c1967a3cfe0718`  
		Last Modified: Sat, 12 Nov 2022 10:03:26 GMT  
		Size: 3.3 MB (3298059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65ea668ec7df7f50f53a7856922aa0885ea15b233b2a8272bd4fbb0375639b1`  
		Last Modified: Wed, 01 Feb 2023 21:44:12 GMT  
		Size: 44.3 MB (44297831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266f21d86884f435a855689439601e152c3345dfb9d9e97d49dfebd93cc82c26`  
		Last Modified: Wed, 01 Feb 2023 21:44:04 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.24.4`

```console
$ docker pull telegraf@sha256:83a43b1251f4e7ff0083e6e9a4414a5e513b57cb276236cbf6d08cd661b4f825
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.24.4` - linux; amd64

```console
$ docker pull telegraf@sha256:219891c4a0aec028e69d393f8149d652c054e051723aa8d336ab29926ce263e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134296996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a4580474fe8c87144e34d00df2b5e3afcd0f9c592f00c5cf9ed4c897c7c740b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:26 GMT
ADD file:cc6a56676703ec7ab5db8f2f7bc18a3169c0816d38703845b6b77ae5342ab41c in / 
# Sat, 04 Feb 2023 06:51:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:22:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:22:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 05 Feb 2023 00:17:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 00:17:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 05 Feb 2023 00:17:26 GMT
ENV TELEGRAF_VERSION=1.24.4
# Sun, 05 Feb 2023 00:17:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sun, 05 Feb 2023 00:17:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sun, 05 Feb 2023 00:17:36 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sun, 05 Feb 2023 00:17:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 05 Feb 2023 00:17:36 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:699c8a97647f5789e5850bcf1a3d5afe9730edb654e1ae0714d5bd198a67a3ed`  
		Last Modified: Sat, 04 Feb 2023 06:55:53 GMT  
		Size: 55.0 MB (55025312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cd158b89fde67a8a4c428a844985f930eba450ec3fde1c9ef5df3884128c62`  
		Last Modified: Sat, 04 Feb 2023 07:29:25 GMT  
		Size: 5.2 MB (5165476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226e961cfaa2d1d171e429e9db314feec6201f5cba1487b20e7aee311e4a54f`  
		Last Modified: Sat, 04 Feb 2023 07:29:25 GMT  
		Size: 10.9 MB (10876697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57437773f0bea58cfa95e8754b53e61f4b2a0a91db902a4b6889886bbd32379f`  
		Last Modified: Sun, 05 Feb 2023 00:18:10 GMT  
		Size: 18.8 MB (18759957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578db7ef68ed573b90f714e49ff85d02b23dc49a904a5a56d51cbff9a5466897`  
		Last Modified: Sun, 05 Feb 2023 00:18:07 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8da18d6a92cc4833971872cba24e8a14a30fa846dd0ea80a1b66d422bc5ef76`  
		Last Modified: Sun, 05 Feb 2023 00:18:30 GMT  
		Size: 44.5 MB (44467403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab8e296304a24b6ebbe650fb626a2f434a8a769b7b62d08a650509cb0f8835c`  
		Last Modified: Sun, 05 Feb 2023 00:18:23 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.24.4` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:5586a64413a0f142389d825d78f9c8c827f1e420032841ef4b75c59cc0930174
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124313376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:588c8f7599ada227ecdbb4bc845749e145cd826184dda24210b59a10247d4def`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:19 GMT
ADD file:239b5255d05e0742f381f82fb7cd586fcc6d9a427263238a2be3372c494ae933 in / 
# Sat, 04 Feb 2023 09:59:20 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:49:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:49:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 05 Feb 2023 05:46:36 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 05:46:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 05 Feb 2023 05:46:51 GMT
ENV TELEGRAF_VERSION=1.24.4
# Sun, 05 Feb 2023 05:46:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sun, 05 Feb 2023 05:46:58 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sun, 05 Feb 2023 05:46:58 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sun, 05 Feb 2023 05:46:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 05 Feb 2023 05:46:58 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:7a21a86b3957d8c99250334cfb78c55af4f8c9277f2f1d4abd53d0362f96323d`  
		Last Modified: Sat, 04 Feb 2023 10:05:53 GMT  
		Size: 50.2 MB (50190828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aacc3c746ca1bd99005f184b00ee418e015c2090c72bda638766d9fb93d3f065`  
		Last Modified: Sat, 04 Feb 2023 10:59:08 GMT  
		Size: 4.9 MB (4933374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b393b343e4fb3b92027c4741418a04d6475259ee243fbf036c1be41df98212`  
		Last Modified: Sat, 04 Feb 2023 10:59:09 GMT  
		Size: 10.2 MB (10217742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46cdeffc1bc9c2d2ce2391093aa478f8a199e3acd00a74991621f53f0c78cb0`  
		Last Modified: Sun, 05 Feb 2023 05:47:43 GMT  
		Size: 17.5 MB (17462246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1302093fdb79f487f8a36fe43c509b03e014f5d1dd15a8bb06b8499d2bd57616`  
		Last Modified: Sun, 05 Feb 2023 05:47:39 GMT  
		Size: 1.8 KB (1780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1033819e1423b511d0d29a8c1fdf787feba297133595dea8c51d27275a7cfc4e`  
		Last Modified: Sun, 05 Feb 2023 05:48:05 GMT  
		Size: 41.5 MB (41507061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94bc6045c8e2194ff2542b1417feca4fe8b6da7b5a6884bddb5a94fcc15656e`  
		Last Modified: Sun, 05 Feb 2023 05:47:57 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.24.4` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:fc102f828ca9dc2878b61e68bd31609ba1a29e1ccc1500489a03c4d73bdf77bf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128635017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52bc5498388a6a51559b9772559d5ac3e6040317fee182b3d460947e995486e8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:08:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:08:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 21:12:59 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 21:13:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 09 Feb 2023 21:13:09 GMT
ENV TELEGRAF_VERSION=1.24.4
# Thu, 09 Feb 2023 21:13:12 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 09 Feb 2023 21:13:13 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 09 Feb 2023 21:13:13 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 09 Feb 2023 21:13:13 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 09 Feb 2023 21:13:13 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae98695cf4875b92116a031bcf51736705c39b105be5f240a143935d8370f6`  
		Last Modified: Thu, 09 Feb 2023 09:14:20 GMT  
		Size: 5.2 MB (5152064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a74e69230a5d5ee55fb6baca6fb52404417efd177a2cb03c418d2d0cf599b5`  
		Last Modified: Thu, 09 Feb 2023 09:14:21 GMT  
		Size: 10.9 MB (10873498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a8c92acaa189d96003ac9c932821ad706b110685d6134804937c672a32cfce`  
		Last Modified: Thu, 09 Feb 2023 21:13:38 GMT  
		Size: 18.6 MB (18598477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8453344745624d949ed6cc91b95bf6b64abdcf79c0b29df0cee561116e2780fc`  
		Last Modified: Thu, 09 Feb 2023 21:13:35 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98825686562eec0e4213e16e3734b97e44fa66bc3c69e516e31af1820939f93`  
		Last Modified: Thu, 09 Feb 2023 21:13:54 GMT  
		Size: 40.3 MB (40305460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8318a7b649fffb5e902a0b741a5c54d51ee7b0a6b6715295c031b94293d666b`  
		Last Modified: Thu, 09 Feb 2023 21:13:49 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.24.4-alpine`

```console
$ docker pull telegraf@sha256:02f7d3ef3ec96fb316c46ef8d9edffda3ef9e1a1674064d692405a3a26466267
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.24.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:2b78bb229fea92cbf8d5de4a73fe57786d4c4bf081728782d2c198c750524564
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50402771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be46e026466d0af78f6c9e4f2b822855db451217c037d63684c71c34e80bcc27`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:32:05 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 12 Nov 2022 10:02:29 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 29 Nov 2022 21:43:37 GMT
ENV TELEGRAF_VERSION=1.24.4
# Wed, 01 Feb 2023 21:42:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 01 Feb 2023 21:42:39 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 01 Feb 2023 21:42:39 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 01 Feb 2023 21:42:40 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 21:42:40 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec8c4909872f004bb7fe69291336b9a1be138c76e18c8706b787cce0ddf850c`  
		Last Modified: Sat, 12 Nov 2022 08:32:35 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb65cee31d4b1da1248e34183af68dd614828735af79e4ec9c1967a3cfe0718`  
		Last Modified: Sat, 12 Nov 2022 10:03:26 GMT  
		Size: 3.3 MB (3298059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65ea668ec7df7f50f53a7856922aa0885ea15b233b2a8272bd4fbb0375639b1`  
		Last Modified: Wed, 01 Feb 2023 21:44:12 GMT  
		Size: 44.3 MB (44297831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:266f21d86884f435a855689439601e152c3345dfb9d9e97d49dfebd93cc82c26`  
		Last Modified: Wed, 01 Feb 2023 21:44:04 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25`

```console
$ docker pull telegraf@sha256:7419524c11e444c2007fe4c6bfad465dcbfadbe7c65bf47c42b3e79c8232a0cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.25` - linux; amd64

```console
$ docker pull telegraf@sha256:9550a9abaf0458d626050505e96a11b58396695315134a108fce6e1a5aa62ce0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.2 MB (136221633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8f19c0c72bdd445e775d248cd37e1b7e097313e3d8516be8cfcdaf8f847bb4f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:26 GMT
ADD file:cc6a56676703ec7ab5db8f2f7bc18a3169c0816d38703845b6b77ae5342ab41c in / 
# Sat, 04 Feb 2023 06:51:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:22:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:22:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 05 Feb 2023 00:17:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 00:17:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 05 Feb 2023 00:17:42 GMT
ENV TELEGRAF_VERSION=1.25.1
# Sun, 05 Feb 2023 00:17:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sun, 05 Feb 2023 00:17:47 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sun, 05 Feb 2023 00:17:47 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sun, 05 Feb 2023 00:17:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 05 Feb 2023 00:17:47 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:699c8a97647f5789e5850bcf1a3d5afe9730edb654e1ae0714d5bd198a67a3ed`  
		Last Modified: Sat, 04 Feb 2023 06:55:53 GMT  
		Size: 55.0 MB (55025312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cd158b89fde67a8a4c428a844985f930eba450ec3fde1c9ef5df3884128c62`  
		Last Modified: Sat, 04 Feb 2023 07:29:25 GMT  
		Size: 5.2 MB (5165476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226e961cfaa2d1d171e429e9db314feec6201f5cba1487b20e7aee311e4a54f`  
		Last Modified: Sat, 04 Feb 2023 07:29:25 GMT  
		Size: 10.9 MB (10876697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57437773f0bea58cfa95e8754b53e61f4b2a0a91db902a4b6889886bbd32379f`  
		Last Modified: Sun, 05 Feb 2023 00:18:10 GMT  
		Size: 18.8 MB (18759957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578db7ef68ed573b90f714e49ff85d02b23dc49a904a5a56d51cbff9a5466897`  
		Last Modified: Sun, 05 Feb 2023 00:18:07 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fcbf4cb163b599b0409b3aea61de6f4ad40a19529dbb0ba7da19f7438df410`  
		Last Modified: Sun, 05 Feb 2023 00:18:47 GMT  
		Size: 46.4 MB (46392040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d030ba1cf89f48eb087693f17019db2fabdb86bc54b5719050ff674724f92a9e`  
		Last Modified: Sun, 05 Feb 2023 00:18:40 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:777c1230d639346496e3952dbbbc163739f10b4fe18f60d2f95a2ffc4034217e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.1 MB (126106473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e381c03a5731ff4a4462abbb63c2f82aea6dde23712d17e620a05e5e12018943`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:19 GMT
ADD file:239b5255d05e0742f381f82fb7cd586fcc6d9a427263238a2be3372c494ae933 in / 
# Sat, 04 Feb 2023 09:59:20 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:49:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:49:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 05 Feb 2023 05:46:36 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 05:46:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 05 Feb 2023 05:47:04 GMT
ENV TELEGRAF_VERSION=1.25.1
# Sun, 05 Feb 2023 05:47:10 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sun, 05 Feb 2023 05:47:11 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sun, 05 Feb 2023 05:47:11 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sun, 05 Feb 2023 05:47:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 05 Feb 2023 05:47:11 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:7a21a86b3957d8c99250334cfb78c55af4f8c9277f2f1d4abd53d0362f96323d`  
		Last Modified: Sat, 04 Feb 2023 10:05:53 GMT  
		Size: 50.2 MB (50190828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aacc3c746ca1bd99005f184b00ee418e015c2090c72bda638766d9fb93d3f065`  
		Last Modified: Sat, 04 Feb 2023 10:59:08 GMT  
		Size: 4.9 MB (4933374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b393b343e4fb3b92027c4741418a04d6475259ee243fbf036c1be41df98212`  
		Last Modified: Sat, 04 Feb 2023 10:59:09 GMT  
		Size: 10.2 MB (10217742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46cdeffc1bc9c2d2ce2391093aa478f8a199e3acd00a74991621f53f0c78cb0`  
		Last Modified: Sun, 05 Feb 2023 05:47:43 GMT  
		Size: 17.5 MB (17462246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1302093fdb79f487f8a36fe43c509b03e014f5d1dd15a8bb06b8499d2bd57616`  
		Last Modified: Sun, 05 Feb 2023 05:47:39 GMT  
		Size: 1.8 KB (1780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64f0e8ab276e41cb0db644368bd9eb8c2abefcf84a67b1802e23e4b4a21b926`  
		Last Modified: Sun, 05 Feb 2023 05:48:24 GMT  
		Size: 43.3 MB (43300161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e087d1e4269853c19308f82eb804aa33adbd39a2c3a327ef7096506d14a134`  
		Last Modified: Sun, 05 Feb 2023 05:48:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:ef119eb991bedf39a9d9526f063bcb2645f6d09b5460c3de65bc39cf156c0758
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130392067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44c4d3089ad9507063acb101aacf24310af4e1e035e8417e37a18b8966782724`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:08:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:08:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 21:12:59 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 21:13:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 09 Feb 2023 21:13:16 GMT
ENV TELEGRAF_VERSION=1.25.1
# Thu, 09 Feb 2023 21:13:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 09 Feb 2023 21:13:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 09 Feb 2023 21:13:22 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 09 Feb 2023 21:13:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 09 Feb 2023 21:13:22 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae98695cf4875b92116a031bcf51736705c39b105be5f240a143935d8370f6`  
		Last Modified: Thu, 09 Feb 2023 09:14:20 GMT  
		Size: 5.2 MB (5152064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a74e69230a5d5ee55fb6baca6fb52404417efd177a2cb03c418d2d0cf599b5`  
		Last Modified: Thu, 09 Feb 2023 09:14:21 GMT  
		Size: 10.9 MB (10873498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a8c92acaa189d96003ac9c932821ad706b110685d6134804937c672a32cfce`  
		Last Modified: Thu, 09 Feb 2023 21:13:38 GMT  
		Size: 18.6 MB (18598477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8453344745624d949ed6cc91b95bf6b64abdcf79c0b29df0cee561116e2780fc`  
		Last Modified: Thu, 09 Feb 2023 21:13:35 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0785c53c7fa846cf27b8bfa6f3719d5c39672c50a7a7d4e28415f7932dbb02`  
		Last Modified: Thu, 09 Feb 2023 21:14:08 GMT  
		Size: 42.1 MB (42062510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca70bd9bc6ed94de6e8ff4ecc7e50a2993d0e618acdc883186c6cf16ea6807a8`  
		Last Modified: Thu, 09 Feb 2023 21:14:03 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25-alpine`

```console
$ docker pull telegraf@sha256:d57e21d98c6b025a82b25766503efdb2aa16027611343cc1194b4003bdcb9c7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.25-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:15427dda77b98c6ec6a82f41f00f69feea4b2458e233e53f022a0c26d8276622
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.3 MB (52333357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e68b84e6353ceb6b229600fb542b87a36b435a4a178a5930bd5114535e67ea45`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:32:05 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 12 Nov 2022 10:02:29 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 01 Feb 2023 21:42:52 GMT
ENV TELEGRAF_VERSION=1.25.1
# Wed, 01 Feb 2023 21:42:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 01 Feb 2023 21:42:58 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 01 Feb 2023 21:42:58 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 01 Feb 2023 21:42:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 21:42:58 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec8c4909872f004bb7fe69291336b9a1be138c76e18c8706b787cce0ddf850c`  
		Last Modified: Sat, 12 Nov 2022 08:32:35 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb65cee31d4b1da1248e34183af68dd614828735af79e4ec9c1967a3cfe0718`  
		Last Modified: Sat, 12 Nov 2022 10:03:26 GMT  
		Size: 3.3 MB (3298059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e7285372a06993b2631e1ec788fb2a4fcb5ed08aaf906d133269089f4a16dd`  
		Last Modified: Wed, 01 Feb 2023 21:44:46 GMT  
		Size: 46.2 MB (46228417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805845b9c28f21f3d8930310952d796e96591bfd497d9ad0b7634118aa00fdc5`  
		Last Modified: Wed, 01 Feb 2023 21:44:38 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25.1`

```console
$ docker pull telegraf@sha256:7419524c11e444c2007fe4c6bfad465dcbfadbe7c65bf47c42b3e79c8232a0cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.25.1` - linux; amd64

```console
$ docker pull telegraf@sha256:9550a9abaf0458d626050505e96a11b58396695315134a108fce6e1a5aa62ce0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.2 MB (136221633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8f19c0c72bdd445e775d248cd37e1b7e097313e3d8516be8cfcdaf8f847bb4f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:26 GMT
ADD file:cc6a56676703ec7ab5db8f2f7bc18a3169c0816d38703845b6b77ae5342ab41c in / 
# Sat, 04 Feb 2023 06:51:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:22:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:22:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 05 Feb 2023 00:17:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 00:17:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 05 Feb 2023 00:17:42 GMT
ENV TELEGRAF_VERSION=1.25.1
# Sun, 05 Feb 2023 00:17:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sun, 05 Feb 2023 00:17:47 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sun, 05 Feb 2023 00:17:47 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sun, 05 Feb 2023 00:17:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 05 Feb 2023 00:17:47 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:699c8a97647f5789e5850bcf1a3d5afe9730edb654e1ae0714d5bd198a67a3ed`  
		Last Modified: Sat, 04 Feb 2023 06:55:53 GMT  
		Size: 55.0 MB (55025312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cd158b89fde67a8a4c428a844985f930eba450ec3fde1c9ef5df3884128c62`  
		Last Modified: Sat, 04 Feb 2023 07:29:25 GMT  
		Size: 5.2 MB (5165476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226e961cfaa2d1d171e429e9db314feec6201f5cba1487b20e7aee311e4a54f`  
		Last Modified: Sat, 04 Feb 2023 07:29:25 GMT  
		Size: 10.9 MB (10876697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57437773f0bea58cfa95e8754b53e61f4b2a0a91db902a4b6889886bbd32379f`  
		Last Modified: Sun, 05 Feb 2023 00:18:10 GMT  
		Size: 18.8 MB (18759957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578db7ef68ed573b90f714e49ff85d02b23dc49a904a5a56d51cbff9a5466897`  
		Last Modified: Sun, 05 Feb 2023 00:18:07 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fcbf4cb163b599b0409b3aea61de6f4ad40a19529dbb0ba7da19f7438df410`  
		Last Modified: Sun, 05 Feb 2023 00:18:47 GMT  
		Size: 46.4 MB (46392040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d030ba1cf89f48eb087693f17019db2fabdb86bc54b5719050ff674724f92a9e`  
		Last Modified: Sun, 05 Feb 2023 00:18:40 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25.1` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:777c1230d639346496e3952dbbbc163739f10b4fe18f60d2f95a2ffc4034217e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.1 MB (126106473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e381c03a5731ff4a4462abbb63c2f82aea6dde23712d17e620a05e5e12018943`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:19 GMT
ADD file:239b5255d05e0742f381f82fb7cd586fcc6d9a427263238a2be3372c494ae933 in / 
# Sat, 04 Feb 2023 09:59:20 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:49:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:49:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 05 Feb 2023 05:46:36 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 05:46:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 05 Feb 2023 05:47:04 GMT
ENV TELEGRAF_VERSION=1.25.1
# Sun, 05 Feb 2023 05:47:10 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sun, 05 Feb 2023 05:47:11 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sun, 05 Feb 2023 05:47:11 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sun, 05 Feb 2023 05:47:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 05 Feb 2023 05:47:11 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:7a21a86b3957d8c99250334cfb78c55af4f8c9277f2f1d4abd53d0362f96323d`  
		Last Modified: Sat, 04 Feb 2023 10:05:53 GMT  
		Size: 50.2 MB (50190828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aacc3c746ca1bd99005f184b00ee418e015c2090c72bda638766d9fb93d3f065`  
		Last Modified: Sat, 04 Feb 2023 10:59:08 GMT  
		Size: 4.9 MB (4933374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b393b343e4fb3b92027c4741418a04d6475259ee243fbf036c1be41df98212`  
		Last Modified: Sat, 04 Feb 2023 10:59:09 GMT  
		Size: 10.2 MB (10217742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46cdeffc1bc9c2d2ce2391093aa478f8a199e3acd00a74991621f53f0c78cb0`  
		Last Modified: Sun, 05 Feb 2023 05:47:43 GMT  
		Size: 17.5 MB (17462246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1302093fdb79f487f8a36fe43c509b03e014f5d1dd15a8bb06b8499d2bd57616`  
		Last Modified: Sun, 05 Feb 2023 05:47:39 GMT  
		Size: 1.8 KB (1780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64f0e8ab276e41cb0db644368bd9eb8c2abefcf84a67b1802e23e4b4a21b926`  
		Last Modified: Sun, 05 Feb 2023 05:48:24 GMT  
		Size: 43.3 MB (43300161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e087d1e4269853c19308f82eb804aa33adbd39a2c3a327ef7096506d14a134`  
		Last Modified: Sun, 05 Feb 2023 05:48:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25.1` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:ef119eb991bedf39a9d9526f063bcb2645f6d09b5460c3de65bc39cf156c0758
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130392067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44c4d3089ad9507063acb101aacf24310af4e1e035e8417e37a18b8966782724`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:08:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:08:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 21:12:59 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 21:13:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 09 Feb 2023 21:13:16 GMT
ENV TELEGRAF_VERSION=1.25.1
# Thu, 09 Feb 2023 21:13:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 09 Feb 2023 21:13:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 09 Feb 2023 21:13:22 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 09 Feb 2023 21:13:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 09 Feb 2023 21:13:22 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae98695cf4875b92116a031bcf51736705c39b105be5f240a143935d8370f6`  
		Last Modified: Thu, 09 Feb 2023 09:14:20 GMT  
		Size: 5.2 MB (5152064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a74e69230a5d5ee55fb6baca6fb52404417efd177a2cb03c418d2d0cf599b5`  
		Last Modified: Thu, 09 Feb 2023 09:14:21 GMT  
		Size: 10.9 MB (10873498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a8c92acaa189d96003ac9c932821ad706b110685d6134804937c672a32cfce`  
		Last Modified: Thu, 09 Feb 2023 21:13:38 GMT  
		Size: 18.6 MB (18598477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8453344745624d949ed6cc91b95bf6b64abdcf79c0b29df0cee561116e2780fc`  
		Last Modified: Thu, 09 Feb 2023 21:13:35 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0785c53c7fa846cf27b8bfa6f3719d5c39672c50a7a7d4e28415f7932dbb02`  
		Last Modified: Thu, 09 Feb 2023 21:14:08 GMT  
		Size: 42.1 MB (42062510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca70bd9bc6ed94de6e8ff4ecc7e50a2993d0e618acdc883186c6cf16ea6807a8`  
		Last Modified: Thu, 09 Feb 2023 21:14:03 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25.1-alpine`

```console
$ docker pull telegraf@sha256:d57e21d98c6b025a82b25766503efdb2aa16027611343cc1194b4003bdcb9c7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.25.1-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:15427dda77b98c6ec6a82f41f00f69feea4b2458e233e53f022a0c26d8276622
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.3 MB (52333357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e68b84e6353ceb6b229600fb542b87a36b435a4a178a5930bd5114535e67ea45`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:32:05 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 12 Nov 2022 10:02:29 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 01 Feb 2023 21:42:52 GMT
ENV TELEGRAF_VERSION=1.25.1
# Wed, 01 Feb 2023 21:42:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 01 Feb 2023 21:42:58 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 01 Feb 2023 21:42:58 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 01 Feb 2023 21:42:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 21:42:58 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec8c4909872f004bb7fe69291336b9a1be138c76e18c8706b787cce0ddf850c`  
		Last Modified: Sat, 12 Nov 2022 08:32:35 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb65cee31d4b1da1248e34183af68dd614828735af79e4ec9c1967a3cfe0718`  
		Last Modified: Sat, 12 Nov 2022 10:03:26 GMT  
		Size: 3.3 MB (3298059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e7285372a06993b2631e1ec788fb2a4fcb5ed08aaf906d133269089f4a16dd`  
		Last Modified: Wed, 01 Feb 2023 21:44:46 GMT  
		Size: 46.2 MB (46228417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805845b9c28f21f3d8930310952d796e96591bfd497d9ad0b7634118aa00fdc5`  
		Last Modified: Wed, 01 Feb 2023 21:44:38 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:d57e21d98c6b025a82b25766503efdb2aa16027611343cc1194b4003bdcb9c7d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:15427dda77b98c6ec6a82f41f00f69feea4b2458e233e53f022a0c26d8276622
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.3 MB (52333357 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e68b84e6353ceb6b229600fb542b87a36b435a4a178a5930bd5114535e67ea45`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 12 Nov 2022 04:19:23 GMT
ADD file:ceeb6e8632fafc657116cbf3afbd522185a16963230b57881073dad22eb0e1a3 in / 
# Sat, 12 Nov 2022 04:19:23 GMT
CMD ["/bin/sh"]
# Sat, 12 Nov 2022 08:32:05 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 12 Nov 2022 10:02:29 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 01 Feb 2023 21:42:52 GMT
ENV TELEGRAF_VERSION=1.25.1
# Wed, 01 Feb 2023 21:42:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 01 Feb 2023 21:42:58 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 01 Feb 2023 21:42:58 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 01 Feb 2023 21:42:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 21:42:58 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ca7dd9ec2225f2385955c43b2379305acd51543c28cf1d4e94522b3d94cce3ce`  
		Last Modified: Sat, 12 Nov 2022 02:52:15 GMT  
		Size: 2.8 MB (2806272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec8c4909872f004bb7fe69291336b9a1be138c76e18c8706b787cce0ddf850c`  
		Last Modified: Sat, 12 Nov 2022 08:32:35 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb65cee31d4b1da1248e34183af68dd614828735af79e4ec9c1967a3cfe0718`  
		Last Modified: Sat, 12 Nov 2022 10:03:26 GMT  
		Size: 3.3 MB (3298059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e7285372a06993b2631e1ec788fb2a4fcb5ed08aaf906d133269089f4a16dd`  
		Last Modified: Wed, 01 Feb 2023 21:44:46 GMT  
		Size: 46.2 MB (46228417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805845b9c28f21f3d8930310952d796e96591bfd497d9ad0b7634118aa00fdc5`  
		Last Modified: Wed, 01 Feb 2023 21:44:38 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:7419524c11e444c2007fe4c6bfad465dcbfadbe7c65bf47c42b3e79c8232a0cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:9550a9abaf0458d626050505e96a11b58396695315134a108fce6e1a5aa62ce0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.2 MB (136221633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8f19c0c72bdd445e775d248cd37e1b7e097313e3d8516be8cfcdaf8f847bb4f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:26 GMT
ADD file:cc6a56676703ec7ab5db8f2f7bc18a3169c0816d38703845b6b77ae5342ab41c in / 
# Sat, 04 Feb 2023 06:51:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:22:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:22:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 05 Feb 2023 00:17:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 00:17:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 05 Feb 2023 00:17:42 GMT
ENV TELEGRAF_VERSION=1.25.1
# Sun, 05 Feb 2023 00:17:47 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sun, 05 Feb 2023 00:17:47 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sun, 05 Feb 2023 00:17:47 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sun, 05 Feb 2023 00:17:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 05 Feb 2023 00:17:47 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:699c8a97647f5789e5850bcf1a3d5afe9730edb654e1ae0714d5bd198a67a3ed`  
		Last Modified: Sat, 04 Feb 2023 06:55:53 GMT  
		Size: 55.0 MB (55025312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cd158b89fde67a8a4c428a844985f930eba450ec3fde1c9ef5df3884128c62`  
		Last Modified: Sat, 04 Feb 2023 07:29:25 GMT  
		Size: 5.2 MB (5165476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226e961cfaa2d1d171e429e9db314feec6201f5cba1487b20e7aee311e4a54f`  
		Last Modified: Sat, 04 Feb 2023 07:29:25 GMT  
		Size: 10.9 MB (10876697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57437773f0bea58cfa95e8754b53e61f4b2a0a91db902a4b6889886bbd32379f`  
		Last Modified: Sun, 05 Feb 2023 00:18:10 GMT  
		Size: 18.8 MB (18759957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578db7ef68ed573b90f714e49ff85d02b23dc49a904a5a56d51cbff9a5466897`  
		Last Modified: Sun, 05 Feb 2023 00:18:07 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9fcbf4cb163b599b0409b3aea61de6f4ad40a19529dbb0ba7da19f7438df410`  
		Last Modified: Sun, 05 Feb 2023 00:18:47 GMT  
		Size: 46.4 MB (46392040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d030ba1cf89f48eb087693f17019db2fabdb86bc54b5719050ff674724f92a9e`  
		Last Modified: Sun, 05 Feb 2023 00:18:40 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:777c1230d639346496e3952dbbbc163739f10b4fe18f60d2f95a2ffc4034217e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.1 MB (126106473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e381c03a5731ff4a4462abbb63c2f82aea6dde23712d17e620a05e5e12018943`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:19 GMT
ADD file:239b5255d05e0742f381f82fb7cd586fcc6d9a427263238a2be3372c494ae933 in / 
# Sat, 04 Feb 2023 09:59:20 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:49:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:49:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 05 Feb 2023 05:46:36 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 05:46:38 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sun, 05 Feb 2023 05:47:04 GMT
ENV TELEGRAF_VERSION=1.25.1
# Sun, 05 Feb 2023 05:47:10 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sun, 05 Feb 2023 05:47:11 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sun, 05 Feb 2023 05:47:11 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Sun, 05 Feb 2023 05:47:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sun, 05 Feb 2023 05:47:11 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:7a21a86b3957d8c99250334cfb78c55af4f8c9277f2f1d4abd53d0362f96323d`  
		Last Modified: Sat, 04 Feb 2023 10:05:53 GMT  
		Size: 50.2 MB (50190828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aacc3c746ca1bd99005f184b00ee418e015c2090c72bda638766d9fb93d3f065`  
		Last Modified: Sat, 04 Feb 2023 10:59:08 GMT  
		Size: 4.9 MB (4933374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b393b343e4fb3b92027c4741418a04d6475259ee243fbf036c1be41df98212`  
		Last Modified: Sat, 04 Feb 2023 10:59:09 GMT  
		Size: 10.2 MB (10217742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46cdeffc1bc9c2d2ce2391093aa478f8a199e3acd00a74991621f53f0c78cb0`  
		Last Modified: Sun, 05 Feb 2023 05:47:43 GMT  
		Size: 17.5 MB (17462246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1302093fdb79f487f8a36fe43c509b03e014f5d1dd15a8bb06b8499d2bd57616`  
		Last Modified: Sun, 05 Feb 2023 05:47:39 GMT  
		Size: 1.8 KB (1780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64f0e8ab276e41cb0db644368bd9eb8c2abefcf84a67b1802e23e4b4a21b926`  
		Last Modified: Sun, 05 Feb 2023 05:48:24 GMT  
		Size: 43.3 MB (43300161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e087d1e4269853c19308f82eb804aa33adbd39a2c3a327ef7096506d14a134`  
		Last Modified: Sun, 05 Feb 2023 05:48:16 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:ef119eb991bedf39a9d9526f063bcb2645f6d09b5460c3de65bc39cf156c0758
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130392067 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44c4d3089ad9507063acb101aacf24310af4e1e035e8417e37a18b8966782724`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:29 GMT
ADD file:5cf2de182dac36d99ec41918889c9755f9c49c56fa0a8d0ca14040c1d8c04541 in / 
# Thu, 09 Feb 2023 03:58:30 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 09:08:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 09:08:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 09 Feb 2023 21:12:59 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 21:13:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 09 Feb 2023 21:13:16 GMT
ENV TELEGRAF_VERSION=1.25.1
# Thu, 09 Feb 2023 21:13:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 09 Feb 2023 21:13:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 09 Feb 2023 21:13:22 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 09 Feb 2023 21:13:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 09 Feb 2023 21:13:22 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:80dae1b9d879348c210c40024c6e90ef92677ac3515456375fcbb70bdf07b104`  
		Last Modified: Thu, 09 Feb 2023 04:02:11 GMT  
		Size: 53.7 MB (53703368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13ae98695cf4875b92116a031bcf51736705c39b105be5f240a143935d8370f6`  
		Last Modified: Thu, 09 Feb 2023 09:14:20 GMT  
		Size: 5.2 MB (5152064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a74e69230a5d5ee55fb6baca6fb52404417efd177a2cb03c418d2d0cf599b5`  
		Last Modified: Thu, 09 Feb 2023 09:14:21 GMT  
		Size: 10.9 MB (10873498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a8c92acaa189d96003ac9c932821ad706b110685d6134804937c672a32cfce`  
		Last Modified: Thu, 09 Feb 2023 21:13:38 GMT  
		Size: 18.6 MB (18598477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8453344745624d949ed6cc91b95bf6b64abdcf79c0b29df0cee561116e2780fc`  
		Last Modified: Thu, 09 Feb 2023 21:13:35 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0785c53c7fa846cf27b8bfa6f3719d5c39672c50a7a7d4e28415f7932dbb02`  
		Last Modified: Thu, 09 Feb 2023 21:14:08 GMT  
		Size: 42.1 MB (42062510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca70bd9bc6ed94de6e8ff4ecc7e50a2993d0e618acdc883186c6cf16ea6807a8`  
		Last Modified: Thu, 09 Feb 2023 21:14:03 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
