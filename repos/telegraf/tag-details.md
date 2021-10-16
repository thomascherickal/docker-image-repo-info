<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `telegraf`

-	[`telegraf:1.18`](#telegraf118)
-	[`telegraf:1.18-alpine`](#telegraf118-alpine)
-	[`telegraf:1.18.3`](#telegraf1183)
-	[`telegraf:1.18.3-alpine`](#telegraf1183-alpine)
-	[`telegraf:1.19`](#telegraf119)
-	[`telegraf:1.19-alpine`](#telegraf119-alpine)
-	[`telegraf:1.19.3`](#telegraf1193)
-	[`telegraf:1.19.3-alpine`](#telegraf1193-alpine)
-	[`telegraf:1.20`](#telegraf120)
-	[`telegraf:1.20-alpine`](#telegraf120-alpine)
-	[`telegraf:1.20.2`](#telegraf1202)
-	[`telegraf:1.20.2-alpine`](#telegraf1202-alpine)
-	[`telegraf:alpine`](#telegrafalpine)
-	[`telegraf:latest`](#telegraflatest)

## `telegraf:1.18`

```console
$ docker pull telegraf@sha256:f2720904f3b4456086140a317817398d484a0229e154fc03ca8d3c39ecb75b7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.18` - linux; amd64

```console
$ docker pull telegraf@sha256:c1f6f1ec54e4a5a221a812767a83ce8e64d447839dde9cf796b2fef287549013
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115493923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:820fcde439e96305f1f97e9e9a22a7138a364efccbc6e60256757fab83fab4a2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:44:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:44:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Oct 2021 10:25:38 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 10:25:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 13 Oct 2021 10:25:46 GMT
ENV TELEGRAF_VERSION=1.18.3
# Wed, 13 Oct 2021 10:26:08 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 13 Oct 2021 10:26:08 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 13 Oct 2021 10:26:08 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 13 Oct 2021 10:26:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 10:26:09 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cef1aa2170c001b320769bf8b018ed82d2c94a673e3010ea1ffe152e107419`  
		Last Modified: Tue, 12 Oct 2021 15:54:16 GMT  
		Size: 7.8 MB (7833862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a51f13be8e69cfc526b671d0bbf621b985b0932acd1523050e2995777b5926`  
		Last Modified: Tue, 12 Oct 2021 15:54:17 GMT  
		Size: 10.0 MB (9997204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c91a466291d423e3faad6a8be6ae82e4a4d0550acb67989ac71c98f900e74d41`  
		Last Modified: Wed, 13 Oct 2021 10:26:55 GMT  
		Size: 17.4 MB (17415387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77934da0dce5bef46b239a3871787c2962a08cf1c8b1e629282f0c617b46426`  
		Last Modified: Wed, 13 Oct 2021 10:26:52 GMT  
		Size: 2.9 KB (2906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3dc5b173c6a2c70c8525fe530dc15fba03195a14a25a922d13d3a4907d3bb79`  
		Last Modified: Wed, 13 Oct 2021 10:26:58 GMT  
		Size: 29.8 MB (29807686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cf876860396d56f47ee7212279da8a2b180793991d68230840f23dabb28e23`  
		Last Modified: Wed, 13 Oct 2021 10:26:52 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.18` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:21e7b0499859364763d5aa8a43aca56835fb9e03a5e2296450f7c77cc5764c66
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.1 MB (106106512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a0f21152146f647d958187ef09e0ee24ad2194fc5db82bd2fc69b2003316674`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:06 GMT
ADD file:b1857dc4fe4fbc4af220829cc6af7169c4555d3f63a3a304db6fa0146b1d5539 in / 
# Tue, 12 Oct 2021 01:29:08 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:39:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:39:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Oct 2021 15:31:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 15:31:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 13 Oct 2021 15:31:08 GMT
ENV TELEGRAF_VERSION=1.18.3
# Wed, 13 Oct 2021 15:31:18 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 13 Oct 2021 15:31:19 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 13 Oct 2021 15:31:20 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 13 Oct 2021 15:31:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 15:31:20 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:139a906e9407e96c50669130c30fe8fba2681b14aa838a3e52f8753b566ef1c8`  
		Last Modified: Tue, 12 Oct 2021 01:45:13 GMT  
		Size: 45.9 MB (45917899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3907051e2154d5bd4ad15141b8938bc09674039787512494a99b93fd4ebc088d`  
		Last Modified: Tue, 12 Oct 2021 19:00:49 GMT  
		Size: 7.1 MB (7125242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8651d4793d5f4d465002213d2d462c964aaf8665a87d5f9cc0de7384f10eeb10`  
		Last Modified: Tue, 12 Oct 2021 19:00:49 GMT  
		Size: 9.3 MB (9343819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e659684a04aace7b984a69bccde2a720cb53304f8905d65b9068605177b2a4b6`  
		Last Modified: Wed, 13 Oct 2021 15:33:06 GMT  
		Size: 16.2 MB (16161376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc86d346babddcb58c40b9188fc289d120a16518eed1782662459497e55f179`  
		Last Modified: Wed, 13 Oct 2021 15:32:54 GMT  
		Size: 2.9 KB (2905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e892c3ebef241bd086d8580d87fe9e607dcddc9648567b441ee73ee6c8ec9`  
		Last Modified: Wed, 13 Oct 2021 15:33:13 GMT  
		Size: 27.6 MB (27555085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2d42d1be45b8bf2cfd8eff5a6ab3c459fe181d9b92d15fb7c9d3784aa9f1b3`  
		Last Modified: Wed, 13 Oct 2021 15:32:54 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.18` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:86d0ac50ccadefe5472953c0bac7dde4a97dff5e23ba4023b44d0adc503caa29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110720290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:536a4c593d6bf0414ffb567d70286e33f6074a9f61be239e7a5edae44c9fc345`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:28 GMT
ADD file:aed1709ccba6a81b9726b228fad7b81bcf4c16bafe723981ad37076322d78986 in / 
# Tue, 12 Oct 2021 01:41:29 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:59:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:59:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 11:51:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 11:51:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 16 Oct 2021 11:51:08 GMT
ENV TELEGRAF_VERSION=1.18.3
# Sat, 16 Oct 2021 11:51:12 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sat, 16 Oct 2021 11:51:13 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 16 Oct 2021 11:51:14 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Sat, 16 Oct 2021 11:51:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Oct 2021 11:51:15 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:2ff6d7a9e7d73e4a01b9417518d18c001728c45fa8109ed8f55aaa50e7981482`  
		Last Modified: Tue, 12 Oct 2021 01:48:38 GMT  
		Size: 49.2 MB (49222756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7324ea4098419bc5fa2ac5a138522230bf12cef3996d1740dd00f9d4737d004`  
		Last Modified: Sat, 16 Oct 2021 03:15:37 GMT  
		Size: 7.7 MB (7695063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e213c33a07316d84d829be685bd3b02e1e2bc135f7748c932050e6ed6a3a0d3`  
		Last Modified: Sat, 16 Oct 2021 03:15:37 GMT  
		Size: 9.8 MB (9767289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195fcb7c5d1eb571a72b8f9d97c3baa030a716aa837f3e8228435b153a518cca`  
		Last Modified: Sat, 16 Oct 2021 11:52:14 GMT  
		Size: 17.1 MB (17058985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb3a6b78fdf159f9ca6b70db784a6eafd05eb4f5f46555df56c6d48d032c608`  
		Last Modified: Sat, 16 Oct 2021 11:52:11 GMT  
		Size: 2.9 KB (2879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e882748fd14001237e38063bb3983a9ad85c8a53ec3b58b5a091f8315d8224`  
		Last Modified: Sat, 16 Oct 2021 11:52:16 GMT  
		Size: 27.0 MB (26973134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c37e8a900b7ea32e9f9938a491628e8844db5bf358d3902372c628daaed4c7`  
		Last Modified: Sat, 16 Oct 2021 11:52:11 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.18-alpine`

```console
$ docker pull telegraf@sha256:54f7d95710bec6be6dbfd34f9ececa44f7a62625ddf08cc8a19a3a8c9daea4fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.18-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:a5ed2c3525bbcac419ff4106559111b23262d1dcf2d4442131f61e59c0c6762c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.8 MB (35825520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c61fd8347299fcbd229c84225f1848893b8befb9b10c5e509f06acc30cc0b0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 20 Sep 2021 22:24:35 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Mon, 20 Sep 2021 22:24:35 GMT
ENV TELEGRAF_VERSION=1.18.3
# Mon, 20 Sep 2021 22:24:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 20 Sep 2021 22:24:47 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 20 Sep 2021 22:24:47 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Mon, 20 Sep 2021 22:24:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Sep 2021 22:24:47 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758daa9673013581700790c0ac7a9855a70445ef1c41bfc2d0ab94288ab13a6b`  
		Last Modified: Mon, 20 Sep 2021 22:25:51 GMT  
		Size: 3.3 MB (3348558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761107a7940fcf466d1539a328a172e7e7df5f60feaa041ec0cc2755ba40c02a`  
		Last Modified: Mon, 20 Sep 2021 22:25:56 GMT  
		Size: 29.7 MB (29662183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be8707dbd19b7008501e669c7515732e124b8f9a93989a739b4a4bb87dfffc5`  
		Last Modified: Mon, 20 Sep 2021 22:25:50 GMT  
		Size: 180.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.18.3`

```console
$ docker pull telegraf@sha256:f2720904f3b4456086140a317817398d484a0229e154fc03ca8d3c39ecb75b7a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.18.3` - linux; amd64

```console
$ docker pull telegraf@sha256:c1f6f1ec54e4a5a221a812767a83ce8e64d447839dde9cf796b2fef287549013
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115493923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:820fcde439e96305f1f97e9e9a22a7138a364efccbc6e60256757fab83fab4a2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:44:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:44:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Oct 2021 10:25:38 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 10:25:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 13 Oct 2021 10:25:46 GMT
ENV TELEGRAF_VERSION=1.18.3
# Wed, 13 Oct 2021 10:26:08 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 13 Oct 2021 10:26:08 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 13 Oct 2021 10:26:08 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 13 Oct 2021 10:26:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 10:26:09 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cef1aa2170c001b320769bf8b018ed82d2c94a673e3010ea1ffe152e107419`  
		Last Modified: Tue, 12 Oct 2021 15:54:16 GMT  
		Size: 7.8 MB (7833862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a51f13be8e69cfc526b671d0bbf621b985b0932acd1523050e2995777b5926`  
		Last Modified: Tue, 12 Oct 2021 15:54:17 GMT  
		Size: 10.0 MB (9997204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c91a466291d423e3faad6a8be6ae82e4a4d0550acb67989ac71c98f900e74d41`  
		Last Modified: Wed, 13 Oct 2021 10:26:55 GMT  
		Size: 17.4 MB (17415387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77934da0dce5bef46b239a3871787c2962a08cf1c8b1e629282f0c617b46426`  
		Last Modified: Wed, 13 Oct 2021 10:26:52 GMT  
		Size: 2.9 KB (2906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3dc5b173c6a2c70c8525fe530dc15fba03195a14a25a922d13d3a4907d3bb79`  
		Last Modified: Wed, 13 Oct 2021 10:26:58 GMT  
		Size: 29.8 MB (29807686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36cf876860396d56f47ee7212279da8a2b180793991d68230840f23dabb28e23`  
		Last Modified: Wed, 13 Oct 2021 10:26:52 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.18.3` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:21e7b0499859364763d5aa8a43aca56835fb9e03a5e2296450f7c77cc5764c66
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.1 MB (106106512 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a0f21152146f647d958187ef09e0ee24ad2194fc5db82bd2fc69b2003316674`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:06 GMT
ADD file:b1857dc4fe4fbc4af220829cc6af7169c4555d3f63a3a304db6fa0146b1d5539 in / 
# Tue, 12 Oct 2021 01:29:08 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:39:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:39:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Oct 2021 15:31:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 15:31:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 13 Oct 2021 15:31:08 GMT
ENV TELEGRAF_VERSION=1.18.3
# Wed, 13 Oct 2021 15:31:18 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 13 Oct 2021 15:31:19 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 13 Oct 2021 15:31:20 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 13 Oct 2021 15:31:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 15:31:20 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:139a906e9407e96c50669130c30fe8fba2681b14aa838a3e52f8753b566ef1c8`  
		Last Modified: Tue, 12 Oct 2021 01:45:13 GMT  
		Size: 45.9 MB (45917899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3907051e2154d5bd4ad15141b8938bc09674039787512494a99b93fd4ebc088d`  
		Last Modified: Tue, 12 Oct 2021 19:00:49 GMT  
		Size: 7.1 MB (7125242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8651d4793d5f4d465002213d2d462c964aaf8665a87d5f9cc0de7384f10eeb10`  
		Last Modified: Tue, 12 Oct 2021 19:00:49 GMT  
		Size: 9.3 MB (9343819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e659684a04aace7b984a69bccde2a720cb53304f8905d65b9068605177b2a4b6`  
		Last Modified: Wed, 13 Oct 2021 15:33:06 GMT  
		Size: 16.2 MB (16161376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc86d346babddcb58c40b9188fc289d120a16518eed1782662459497e55f179`  
		Last Modified: Wed, 13 Oct 2021 15:32:54 GMT  
		Size: 2.9 KB (2905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9e892c3ebef241bd086d8580d87fe9e607dcddc9648567b441ee73ee6c8ec9`  
		Last Modified: Wed, 13 Oct 2021 15:33:13 GMT  
		Size: 27.6 MB (27555085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2d42d1be45b8bf2cfd8eff5a6ab3c459fe181d9b92d15fb7c9d3784aa9f1b3`  
		Last Modified: Wed, 13 Oct 2021 15:32:54 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.18.3` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:86d0ac50ccadefe5472953c0bac7dde4a97dff5e23ba4023b44d0adc503caa29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.7 MB (110720290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:536a4c593d6bf0414ffb567d70286e33f6074a9f61be239e7a5edae44c9fc345`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:28 GMT
ADD file:aed1709ccba6a81b9726b228fad7b81bcf4c16bafe723981ad37076322d78986 in / 
# Tue, 12 Oct 2021 01:41:29 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:59:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:59:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 11:51:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 11:51:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 16 Oct 2021 11:51:08 GMT
ENV TELEGRAF_VERSION=1.18.3
# Sat, 16 Oct 2021 11:51:12 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sat, 16 Oct 2021 11:51:13 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 16 Oct 2021 11:51:14 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Sat, 16 Oct 2021 11:51:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Oct 2021 11:51:15 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:2ff6d7a9e7d73e4a01b9417518d18c001728c45fa8109ed8f55aaa50e7981482`  
		Last Modified: Tue, 12 Oct 2021 01:48:38 GMT  
		Size: 49.2 MB (49222756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7324ea4098419bc5fa2ac5a138522230bf12cef3996d1740dd00f9d4737d004`  
		Last Modified: Sat, 16 Oct 2021 03:15:37 GMT  
		Size: 7.7 MB (7695063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e213c33a07316d84d829be685bd3b02e1e2bc135f7748c932050e6ed6a3a0d3`  
		Last Modified: Sat, 16 Oct 2021 03:15:37 GMT  
		Size: 9.8 MB (9767289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195fcb7c5d1eb571a72b8f9d97c3baa030a716aa837f3e8228435b153a518cca`  
		Last Modified: Sat, 16 Oct 2021 11:52:14 GMT  
		Size: 17.1 MB (17058985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb3a6b78fdf159f9ca6b70db784a6eafd05eb4f5f46555df56c6d48d032c608`  
		Last Modified: Sat, 16 Oct 2021 11:52:11 GMT  
		Size: 2.9 KB (2879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e882748fd14001237e38063bb3983a9ad85c8a53ec3b58b5a091f8315d8224`  
		Last Modified: Sat, 16 Oct 2021 11:52:16 GMT  
		Size: 27.0 MB (26973134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c37e8a900b7ea32e9f9938a491628e8844db5bf358d3902372c628daaed4c7`  
		Last Modified: Sat, 16 Oct 2021 11:52:11 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.18.3-alpine`

```console
$ docker pull telegraf@sha256:54f7d95710bec6be6dbfd34f9ececa44f7a62625ddf08cc8a19a3a8c9daea4fd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.18.3-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:a5ed2c3525bbcac419ff4106559111b23262d1dcf2d4442131f61e59c0c6762c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.8 MB (35825520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c61fd8347299fcbd229c84225f1848893b8befb9b10c5e509f06acc30cc0b0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 20 Sep 2021 22:24:35 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Mon, 20 Sep 2021 22:24:35 GMT
ENV TELEGRAF_VERSION=1.18.3
# Mon, 20 Sep 2021 22:24:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 20 Sep 2021 22:24:47 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 20 Sep 2021 22:24:47 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Mon, 20 Sep 2021 22:24:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Sep 2021 22:24:47 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758daa9673013581700790c0ac7a9855a70445ef1c41bfc2d0ab94288ab13a6b`  
		Last Modified: Mon, 20 Sep 2021 22:25:51 GMT  
		Size: 3.3 MB (3348558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:761107a7940fcf466d1539a328a172e7e7df5f60feaa041ec0cc2755ba40c02a`  
		Last Modified: Mon, 20 Sep 2021 22:25:56 GMT  
		Size: 29.7 MB (29662183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be8707dbd19b7008501e669c7515732e124b8f9a93989a739b4a4bb87dfffc5`  
		Last Modified: Mon, 20 Sep 2021 22:25:50 GMT  
		Size: 180.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.19`

```console
$ docker pull telegraf@sha256:54c86019de7e1f7aafd161eefa78fe2617244131b46ff99d3b5e69638dc3884e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.19` - linux; amd64

```console
$ docker pull telegraf@sha256:82bf008303f325ee9f93e5fa7f73fa6f5b2dfbe727c6654d4ee9c40666957b49
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119874069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96797d7b4f447ee34a37dd9b51f4182bfae69329d7feee6cc696349db939117`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:44:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:44:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Oct 2021 10:25:38 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 10:25:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 13 Oct 2021 10:26:13 GMT
ENV TELEGRAF_VERSION=1.19.3
# Wed, 13 Oct 2021 10:26:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 13 Oct 2021 10:26:19 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 13 Oct 2021 10:26:19 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 13 Oct 2021 10:26:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 10:26:20 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cef1aa2170c001b320769bf8b018ed82d2c94a673e3010ea1ffe152e107419`  
		Last Modified: Tue, 12 Oct 2021 15:54:16 GMT  
		Size: 7.8 MB (7833862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a51f13be8e69cfc526b671d0bbf621b985b0932acd1523050e2995777b5926`  
		Last Modified: Tue, 12 Oct 2021 15:54:17 GMT  
		Size: 10.0 MB (9997204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c91a466291d423e3faad6a8be6ae82e4a4d0550acb67989ac71c98f900e74d41`  
		Last Modified: Wed, 13 Oct 2021 10:26:55 GMT  
		Size: 17.4 MB (17415387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77934da0dce5bef46b239a3871787c2962a08cf1c8b1e629282f0c617b46426`  
		Last Modified: Wed, 13 Oct 2021 10:26:52 GMT  
		Size: 2.9 KB (2906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ee4b64760022ecef81a94e508ebef6be4908cf720ddf4638226c3a4e18f01`  
		Last Modified: Wed, 13 Oct 2021 10:27:15 GMT  
		Size: 34.2 MB (34187833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df923ebeb98a14c1029c4a6eac7014c37f02865b8d21a72fdc078394f6b894d`  
		Last Modified: Wed, 13 Oct 2021 10:27:08 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.19` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:6ce1724361b80e2293416f10fc0928296c1ed3b55348a9d85448a37ed991d0dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110245992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:765debeb47dbe4c1ae8c86819e473b5ce9877c2946a7d43316a4ad220b80f035`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:06 GMT
ADD file:b1857dc4fe4fbc4af220829cc6af7169c4555d3f63a3a304db6fa0146b1d5539 in / 
# Tue, 12 Oct 2021 01:29:08 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:39:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:39:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Oct 2021 15:31:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 15:31:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 13 Oct 2021 15:31:32 GMT
ENV TELEGRAF_VERSION=1.19.3
# Wed, 13 Oct 2021 15:31:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 13 Oct 2021 15:31:44 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 13 Oct 2021 15:31:45 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 13 Oct 2021 15:31:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 15:31:45 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:139a906e9407e96c50669130c30fe8fba2681b14aa838a3e52f8753b566ef1c8`  
		Last Modified: Tue, 12 Oct 2021 01:45:13 GMT  
		Size: 45.9 MB (45917899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3907051e2154d5bd4ad15141b8938bc09674039787512494a99b93fd4ebc088d`  
		Last Modified: Tue, 12 Oct 2021 19:00:49 GMT  
		Size: 7.1 MB (7125242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8651d4793d5f4d465002213d2d462c964aaf8665a87d5f9cc0de7384f10eeb10`  
		Last Modified: Tue, 12 Oct 2021 19:00:49 GMT  
		Size: 9.3 MB (9343819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e659684a04aace7b984a69bccde2a720cb53304f8905d65b9068605177b2a4b6`  
		Last Modified: Wed, 13 Oct 2021 15:33:06 GMT  
		Size: 16.2 MB (16161376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc86d346babddcb58c40b9188fc289d120a16518eed1782662459497e55f179`  
		Last Modified: Wed, 13 Oct 2021 15:32:54 GMT  
		Size: 2.9 KB (2905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f9213a7b1180f7eb074ebc32c7adc9824c55705bacd59a5e64ceacc7720b3b`  
		Last Modified: Wed, 13 Oct 2021 15:33:47 GMT  
		Size: 31.7 MB (31694568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddecb98396f812a3a9ba35dff0793776e695181f8dafecd495e11cbf03d6047b`  
		Last Modified: Wed, 13 Oct 2021 15:33:25 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.19` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:62fe6b27709c7a3549000744d004571ea81605c9f60372611585a79ddbffe39e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114713622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec5280d8da660d0c575ecf44463153e15b07159a9f03cdbf44669020e9a66d2e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:28 GMT
ADD file:aed1709ccba6a81b9726b228fad7b81bcf4c16bafe723981ad37076322d78986 in / 
# Tue, 12 Oct 2021 01:41:29 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:59:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:59:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 11:51:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 11:51:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 16 Oct 2021 11:51:23 GMT
ENV TELEGRAF_VERSION=1.19.3
# Sat, 16 Oct 2021 11:51:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sat, 16 Oct 2021 11:51:27 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 16 Oct 2021 11:51:29 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Sat, 16 Oct 2021 11:51:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Oct 2021 11:51:30 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:2ff6d7a9e7d73e4a01b9417518d18c001728c45fa8109ed8f55aaa50e7981482`  
		Last Modified: Tue, 12 Oct 2021 01:48:38 GMT  
		Size: 49.2 MB (49222756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7324ea4098419bc5fa2ac5a138522230bf12cef3996d1740dd00f9d4737d004`  
		Last Modified: Sat, 16 Oct 2021 03:15:37 GMT  
		Size: 7.7 MB (7695063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e213c33a07316d84d829be685bd3b02e1e2bc135f7748c932050e6ed6a3a0d3`  
		Last Modified: Sat, 16 Oct 2021 03:15:37 GMT  
		Size: 9.8 MB (9767289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195fcb7c5d1eb571a72b8f9d97c3baa030a716aa837f3e8228435b153a518cca`  
		Last Modified: Sat, 16 Oct 2021 11:52:14 GMT  
		Size: 17.1 MB (17058985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb3a6b78fdf159f9ca6b70db784a6eafd05eb4f5f46555df56c6d48d032c608`  
		Last Modified: Sat, 16 Oct 2021 11:52:11 GMT  
		Size: 2.9 KB (2879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d521ff76d5175010c3864c432ab662004079fd9bd5b37d02ddae4899af4c0e`  
		Last Modified: Sat, 16 Oct 2021 11:52:32 GMT  
		Size: 31.0 MB (30966464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64278d5086c58b520e36feeb70213fe3a3c70f9dc29731da01922c40b26c4d8`  
		Last Modified: Sat, 16 Oct 2021 11:52:26 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.19-alpine`

```console
$ docker pull telegraf@sha256:2e65a6535cb8c75c9d7f20e51ce88f09357fc6dc2ffe41175b31e45c3efda436
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.19-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:74026098b03c0987ac7fd188500a426f43b4154c9311295f4c250cbe1e69a8bc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40206011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:970d4a14426e879dc556179d3a30bfc2cdf3b84b85333c6f9fc0c81f154b5405`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 20 Sep 2021 22:24:35 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Mon, 20 Sep 2021 22:24:55 GMT
ENV TELEGRAF_VERSION=1.19.3
# Mon, 20 Sep 2021 22:25:04 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 20 Sep 2021 22:25:04 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 20 Sep 2021 22:25:05 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Mon, 20 Sep 2021 22:25:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Sep 2021 22:25:05 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758daa9673013581700790c0ac7a9855a70445ef1c41bfc2d0ab94288ab13a6b`  
		Last Modified: Mon, 20 Sep 2021 22:25:51 GMT  
		Size: 3.3 MB (3348558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955fdac0c850f29f7b887fcd1db8f08b605774d344acd055d0e1fb9a20345bc9`  
		Last Modified: Mon, 20 Sep 2021 22:26:13 GMT  
		Size: 34.0 MB (34042670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8079785e70c639292f3dce1274c309b164c689ca2f7473940f557764de4fe5`  
		Last Modified: Mon, 20 Sep 2021 22:26:07 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.19.3`

```console
$ docker pull telegraf@sha256:54c86019de7e1f7aafd161eefa78fe2617244131b46ff99d3b5e69638dc3884e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.19.3` - linux; amd64

```console
$ docker pull telegraf@sha256:82bf008303f325ee9f93e5fa7f73fa6f5b2dfbe727c6654d4ee9c40666957b49
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119874069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a96797d7b4f447ee34a37dd9b51f4182bfae69329d7feee6cc696349db939117`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:44:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:44:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Oct 2021 10:25:38 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 10:25:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 13 Oct 2021 10:26:13 GMT
ENV TELEGRAF_VERSION=1.19.3
# Wed, 13 Oct 2021 10:26:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 13 Oct 2021 10:26:19 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 13 Oct 2021 10:26:19 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 13 Oct 2021 10:26:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 10:26:20 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cef1aa2170c001b320769bf8b018ed82d2c94a673e3010ea1ffe152e107419`  
		Last Modified: Tue, 12 Oct 2021 15:54:16 GMT  
		Size: 7.8 MB (7833862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a51f13be8e69cfc526b671d0bbf621b985b0932acd1523050e2995777b5926`  
		Last Modified: Tue, 12 Oct 2021 15:54:17 GMT  
		Size: 10.0 MB (9997204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c91a466291d423e3faad6a8be6ae82e4a4d0550acb67989ac71c98f900e74d41`  
		Last Modified: Wed, 13 Oct 2021 10:26:55 GMT  
		Size: 17.4 MB (17415387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77934da0dce5bef46b239a3871787c2962a08cf1c8b1e629282f0c617b46426`  
		Last Modified: Wed, 13 Oct 2021 10:26:52 GMT  
		Size: 2.9 KB (2906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:740ee4b64760022ecef81a94e508ebef6be4908cf720ddf4638226c3a4e18f01`  
		Last Modified: Wed, 13 Oct 2021 10:27:15 GMT  
		Size: 34.2 MB (34187833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df923ebeb98a14c1029c4a6eac7014c37f02865b8d21a72fdc078394f6b894d`  
		Last Modified: Wed, 13 Oct 2021 10:27:08 GMT  
		Size: 185.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.19.3` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:6ce1724361b80e2293416f10fc0928296c1ed3b55348a9d85448a37ed991d0dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110245992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:765debeb47dbe4c1ae8c86819e473b5ce9877c2946a7d43316a4ad220b80f035`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:06 GMT
ADD file:b1857dc4fe4fbc4af220829cc6af7169c4555d3f63a3a304db6fa0146b1d5539 in / 
# Tue, 12 Oct 2021 01:29:08 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:39:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:39:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Oct 2021 15:31:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 15:31:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 13 Oct 2021 15:31:32 GMT
ENV TELEGRAF_VERSION=1.19.3
# Wed, 13 Oct 2021 15:31:43 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 13 Oct 2021 15:31:44 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 13 Oct 2021 15:31:45 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 13 Oct 2021 15:31:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 15:31:45 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:139a906e9407e96c50669130c30fe8fba2681b14aa838a3e52f8753b566ef1c8`  
		Last Modified: Tue, 12 Oct 2021 01:45:13 GMT  
		Size: 45.9 MB (45917899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3907051e2154d5bd4ad15141b8938bc09674039787512494a99b93fd4ebc088d`  
		Last Modified: Tue, 12 Oct 2021 19:00:49 GMT  
		Size: 7.1 MB (7125242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8651d4793d5f4d465002213d2d462c964aaf8665a87d5f9cc0de7384f10eeb10`  
		Last Modified: Tue, 12 Oct 2021 19:00:49 GMT  
		Size: 9.3 MB (9343819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e659684a04aace7b984a69bccde2a720cb53304f8905d65b9068605177b2a4b6`  
		Last Modified: Wed, 13 Oct 2021 15:33:06 GMT  
		Size: 16.2 MB (16161376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc86d346babddcb58c40b9188fc289d120a16518eed1782662459497e55f179`  
		Last Modified: Wed, 13 Oct 2021 15:32:54 GMT  
		Size: 2.9 KB (2905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f9213a7b1180f7eb074ebc32c7adc9824c55705bacd59a5e64ceacc7720b3b`  
		Last Modified: Wed, 13 Oct 2021 15:33:47 GMT  
		Size: 31.7 MB (31694568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddecb98396f812a3a9ba35dff0793776e695181f8dafecd495e11cbf03d6047b`  
		Last Modified: Wed, 13 Oct 2021 15:33:25 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.19.3` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:62fe6b27709c7a3549000744d004571ea81605c9f60372611585a79ddbffe39e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.7 MB (114713622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec5280d8da660d0c575ecf44463153e15b07159a9f03cdbf44669020e9a66d2e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:28 GMT
ADD file:aed1709ccba6a81b9726b228fad7b81bcf4c16bafe723981ad37076322d78986 in / 
# Tue, 12 Oct 2021 01:41:29 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:59:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:59:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 11:51:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 11:51:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 16 Oct 2021 11:51:23 GMT
ENV TELEGRAF_VERSION=1.19.3
# Sat, 16 Oct 2021 11:51:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sat, 16 Oct 2021 11:51:27 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 16 Oct 2021 11:51:29 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Sat, 16 Oct 2021 11:51:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Oct 2021 11:51:30 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:2ff6d7a9e7d73e4a01b9417518d18c001728c45fa8109ed8f55aaa50e7981482`  
		Last Modified: Tue, 12 Oct 2021 01:48:38 GMT  
		Size: 49.2 MB (49222756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7324ea4098419bc5fa2ac5a138522230bf12cef3996d1740dd00f9d4737d004`  
		Last Modified: Sat, 16 Oct 2021 03:15:37 GMT  
		Size: 7.7 MB (7695063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e213c33a07316d84d829be685bd3b02e1e2bc135f7748c932050e6ed6a3a0d3`  
		Last Modified: Sat, 16 Oct 2021 03:15:37 GMT  
		Size: 9.8 MB (9767289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195fcb7c5d1eb571a72b8f9d97c3baa030a716aa837f3e8228435b153a518cca`  
		Last Modified: Sat, 16 Oct 2021 11:52:14 GMT  
		Size: 17.1 MB (17058985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb3a6b78fdf159f9ca6b70db784a6eafd05eb4f5f46555df56c6d48d032c608`  
		Last Modified: Sat, 16 Oct 2021 11:52:11 GMT  
		Size: 2.9 KB (2879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d521ff76d5175010c3864c432ab662004079fd9bd5b37d02ddae4899af4c0e`  
		Last Modified: Sat, 16 Oct 2021 11:52:32 GMT  
		Size: 31.0 MB (30966464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a64278d5086c58b520e36feeb70213fe3a3c70f9dc29731da01922c40b26c4d8`  
		Last Modified: Sat, 16 Oct 2021 11:52:26 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.19.3-alpine`

```console
$ docker pull telegraf@sha256:2e65a6535cb8c75c9d7f20e51ce88f09357fc6dc2ffe41175b31e45c3efda436
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.19.3-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:74026098b03c0987ac7fd188500a426f43b4154c9311295f4c250cbe1e69a8bc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40206011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:970d4a14426e879dc556179d3a30bfc2cdf3b84b85333c6f9fc0c81f154b5405`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 20 Sep 2021 22:24:35 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Mon, 20 Sep 2021 22:24:55 GMT
ENV TELEGRAF_VERSION=1.19.3
# Mon, 20 Sep 2021 22:25:04 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 20 Sep 2021 22:25:04 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 20 Sep 2021 22:25:05 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Mon, 20 Sep 2021 22:25:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 20 Sep 2021 22:25:05 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758daa9673013581700790c0ac7a9855a70445ef1c41bfc2d0ab94288ab13a6b`  
		Last Modified: Mon, 20 Sep 2021 22:25:51 GMT  
		Size: 3.3 MB (3348558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955fdac0c850f29f7b887fcd1db8f08b605774d344acd055d0e1fb9a20345bc9`  
		Last Modified: Mon, 20 Sep 2021 22:26:13 GMT  
		Size: 34.0 MB (34042670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8079785e70c639292f3dce1274c309b164c689ca2f7473940f557764de4fe5`  
		Last Modified: Mon, 20 Sep 2021 22:26:07 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.20`

```console
$ docker pull telegraf@sha256:700b5b8fcb46844a7396265d90f0274ceb2e169a9c354b5629a9f235993bb139
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.20` - linux; amd64

```console
$ docker pull telegraf@sha256:d7de36f6c04825144b45189eba7c0b363ecb08e63a3a7c8572d8dcf1b4eca73d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120438552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e36bdd348ca3bd084087c93bbb35ece214e69dcd1e17d86389e9a9950e6ba4c2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:44:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:44:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Oct 2021 10:25:38 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 10:25:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 13 Oct 2021 10:26:24 GMT
ENV TELEGRAF_VERSION=1.20.2
# Wed, 13 Oct 2021 10:26:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 13 Oct 2021 10:26:28 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 13 Oct 2021 10:26:29 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 13 Oct 2021 10:26:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 10:26:29 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cef1aa2170c001b320769bf8b018ed82d2c94a673e3010ea1ffe152e107419`  
		Last Modified: Tue, 12 Oct 2021 15:54:16 GMT  
		Size: 7.8 MB (7833862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a51f13be8e69cfc526b671d0bbf621b985b0932acd1523050e2995777b5926`  
		Last Modified: Tue, 12 Oct 2021 15:54:17 GMT  
		Size: 10.0 MB (9997204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c91a466291d423e3faad6a8be6ae82e4a4d0550acb67989ac71c98f900e74d41`  
		Last Modified: Wed, 13 Oct 2021 10:26:55 GMT  
		Size: 17.4 MB (17415387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77934da0dce5bef46b239a3871787c2962a08cf1c8b1e629282f0c617b46426`  
		Last Modified: Wed, 13 Oct 2021 10:26:52 GMT  
		Size: 2.9 KB (2906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fe40b78b74cb29485f43d826630febe77421a130fc3a60e984efee2d0cacca`  
		Last Modified: Wed, 13 Oct 2021 10:27:32 GMT  
		Size: 34.8 MB (34752317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b39af786583bce9560759a1517b19efa4b4d9a1a5a9f2613af7358365db368`  
		Last Modified: Wed, 13 Oct 2021 10:27:26 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.20` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:1095e724ff8b62ca04c45c86c617eb7fda3a1949be4a31a97f3a3d6871b5695d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (110968719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6367f3beba90bfac51b16bf4bd246bf3117f537226d643b0ee0267b158a791eb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:06 GMT
ADD file:b1857dc4fe4fbc4af220829cc6af7169c4555d3f63a3a304db6fa0146b1d5539 in / 
# Tue, 12 Oct 2021 01:29:08 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:39:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:39:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Oct 2021 15:31:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 15:31:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 13 Oct 2021 15:31:57 GMT
ENV TELEGRAF_VERSION=1.20.2
# Wed, 13 Oct 2021 15:32:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 13 Oct 2021 15:32:09 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 13 Oct 2021 15:32:10 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 13 Oct 2021 15:32:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 15:32:11 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:139a906e9407e96c50669130c30fe8fba2681b14aa838a3e52f8753b566ef1c8`  
		Last Modified: Tue, 12 Oct 2021 01:45:13 GMT  
		Size: 45.9 MB (45917899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3907051e2154d5bd4ad15141b8938bc09674039787512494a99b93fd4ebc088d`  
		Last Modified: Tue, 12 Oct 2021 19:00:49 GMT  
		Size: 7.1 MB (7125242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8651d4793d5f4d465002213d2d462c964aaf8665a87d5f9cc0de7384f10eeb10`  
		Last Modified: Tue, 12 Oct 2021 19:00:49 GMT  
		Size: 9.3 MB (9343819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e659684a04aace7b984a69bccde2a720cb53304f8905d65b9068605177b2a4b6`  
		Last Modified: Wed, 13 Oct 2021 15:33:06 GMT  
		Size: 16.2 MB (16161376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc86d346babddcb58c40b9188fc289d120a16518eed1782662459497e55f179`  
		Last Modified: Wed, 13 Oct 2021 15:32:54 GMT  
		Size: 2.9 KB (2905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ab61c37e049992dec37a6aba62a2046c0218ac8e88f196d8f297335e469910`  
		Last Modified: Wed, 13 Oct 2021 15:34:22 GMT  
		Size: 32.4 MB (32417295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7392c9c96023c85c1c1c8747fddf4b44295a00702e98de30a55891277c55c92`  
		Last Modified: Wed, 13 Oct 2021 15:33:59 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.20` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:124443ca528ab9e7f9f5f300500ea5b8d98c755c4fe8478a1b577852868ed9ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115377157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb9a2610badae699324accc3e50e52294a936812017ad668eba96b450ae0d06a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:28 GMT
ADD file:aed1709ccba6a81b9726b228fad7b81bcf4c16bafe723981ad37076322d78986 in / 
# Tue, 12 Oct 2021 01:41:29 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:59:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:59:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 11:51:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 11:51:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 16 Oct 2021 11:51:35 GMT
ENV TELEGRAF_VERSION=1.20.2
# Sat, 16 Oct 2021 11:51:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sat, 16 Oct 2021 11:51:45 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 16 Oct 2021 11:51:46 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Sat, 16 Oct 2021 11:51:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Oct 2021 11:51:47 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:2ff6d7a9e7d73e4a01b9417518d18c001728c45fa8109ed8f55aaa50e7981482`  
		Last Modified: Tue, 12 Oct 2021 01:48:38 GMT  
		Size: 49.2 MB (49222756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7324ea4098419bc5fa2ac5a138522230bf12cef3996d1740dd00f9d4737d004`  
		Last Modified: Sat, 16 Oct 2021 03:15:37 GMT  
		Size: 7.7 MB (7695063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e213c33a07316d84d829be685bd3b02e1e2bc135f7748c932050e6ed6a3a0d3`  
		Last Modified: Sat, 16 Oct 2021 03:15:37 GMT  
		Size: 9.8 MB (9767289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195fcb7c5d1eb571a72b8f9d97c3baa030a716aa837f3e8228435b153a518cca`  
		Last Modified: Sat, 16 Oct 2021 11:52:14 GMT  
		Size: 17.1 MB (17058985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb3a6b78fdf159f9ca6b70db784a6eafd05eb4f5f46555df56c6d48d032c608`  
		Last Modified: Sat, 16 Oct 2021 11:52:11 GMT  
		Size: 2.9 KB (2879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523dbbcea8d35ab6f724f5585dbbd270602fb850af02b87b2227b77c5bc6ec4d`  
		Last Modified: Sat, 16 Oct 2021 11:52:47 GMT  
		Size: 31.6 MB (31629999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f604607ffed6f61d8be9837a6e259de4749b98d9a2f384a1c16889e5f320e024`  
		Last Modified: Sat, 16 Oct 2021 11:52:42 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.20-alpine`

```console
$ docker pull telegraf@sha256:a5fac131412fe7078fb4b7d6d8c4edc5016c984c69cbf1ee787ff59ed5d896c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.20-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:884120aaa5b052fcb8727d4def67519b2bb9f697ae20efec50097721abb4a5dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40758696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:135f23862b5d9b6b00e3540179e34be36eb001c54cb5344ed55554a7d73802f7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 20 Sep 2021 22:24:35 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Fri, 08 Oct 2021 17:31:44 GMT
ENV TELEGRAF_VERSION=1.20.2
# Fri, 08 Oct 2021 17:31:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 08 Oct 2021 17:31:56 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 08 Oct 2021 17:31:56 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Fri, 08 Oct 2021 17:31:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Oct 2021 17:31:56 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758daa9673013581700790c0ac7a9855a70445ef1c41bfc2d0ab94288ab13a6b`  
		Last Modified: Mon, 20 Sep 2021 22:25:51 GMT  
		Size: 3.3 MB (3348558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eafdaa25d6c53cc5132e20cbe015727e3bb384607caf6c76ca71f527bfba272`  
		Last Modified: Fri, 08 Oct 2021 17:32:44 GMT  
		Size: 34.6 MB (34595357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d9340b120badda5a4cd2792ac218ece7061af283ead0fbbd6ca756da19a8c2`  
		Last Modified: Fri, 08 Oct 2021 17:32:38 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.20.2`

```console
$ docker pull telegraf@sha256:700b5b8fcb46844a7396265d90f0274ceb2e169a9c354b5629a9f235993bb139
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.20.2` - linux; amd64

```console
$ docker pull telegraf@sha256:d7de36f6c04825144b45189eba7c0b363ecb08e63a3a7c8572d8dcf1b4eca73d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120438552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e36bdd348ca3bd084087c93bbb35ece214e69dcd1e17d86389e9a9950e6ba4c2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:44:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:44:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Oct 2021 10:25:38 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 10:25:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 13 Oct 2021 10:26:24 GMT
ENV TELEGRAF_VERSION=1.20.2
# Wed, 13 Oct 2021 10:26:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 13 Oct 2021 10:26:28 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 13 Oct 2021 10:26:29 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 13 Oct 2021 10:26:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 10:26:29 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cef1aa2170c001b320769bf8b018ed82d2c94a673e3010ea1ffe152e107419`  
		Last Modified: Tue, 12 Oct 2021 15:54:16 GMT  
		Size: 7.8 MB (7833862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a51f13be8e69cfc526b671d0bbf621b985b0932acd1523050e2995777b5926`  
		Last Modified: Tue, 12 Oct 2021 15:54:17 GMT  
		Size: 10.0 MB (9997204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c91a466291d423e3faad6a8be6ae82e4a4d0550acb67989ac71c98f900e74d41`  
		Last Modified: Wed, 13 Oct 2021 10:26:55 GMT  
		Size: 17.4 MB (17415387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77934da0dce5bef46b239a3871787c2962a08cf1c8b1e629282f0c617b46426`  
		Last Modified: Wed, 13 Oct 2021 10:26:52 GMT  
		Size: 2.9 KB (2906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fe40b78b74cb29485f43d826630febe77421a130fc3a60e984efee2d0cacca`  
		Last Modified: Wed, 13 Oct 2021 10:27:32 GMT  
		Size: 34.8 MB (34752317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b39af786583bce9560759a1517b19efa4b4d9a1a5a9f2613af7358365db368`  
		Last Modified: Wed, 13 Oct 2021 10:27:26 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.20.2` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:1095e724ff8b62ca04c45c86c617eb7fda3a1949be4a31a97f3a3d6871b5695d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (110968719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6367f3beba90bfac51b16bf4bd246bf3117f537226d643b0ee0267b158a791eb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:06 GMT
ADD file:b1857dc4fe4fbc4af220829cc6af7169c4555d3f63a3a304db6fa0146b1d5539 in / 
# Tue, 12 Oct 2021 01:29:08 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:39:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:39:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Oct 2021 15:31:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 15:31:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 13 Oct 2021 15:31:57 GMT
ENV TELEGRAF_VERSION=1.20.2
# Wed, 13 Oct 2021 15:32:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 13 Oct 2021 15:32:09 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 13 Oct 2021 15:32:10 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 13 Oct 2021 15:32:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 15:32:11 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:139a906e9407e96c50669130c30fe8fba2681b14aa838a3e52f8753b566ef1c8`  
		Last Modified: Tue, 12 Oct 2021 01:45:13 GMT  
		Size: 45.9 MB (45917899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3907051e2154d5bd4ad15141b8938bc09674039787512494a99b93fd4ebc088d`  
		Last Modified: Tue, 12 Oct 2021 19:00:49 GMT  
		Size: 7.1 MB (7125242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8651d4793d5f4d465002213d2d462c964aaf8665a87d5f9cc0de7384f10eeb10`  
		Last Modified: Tue, 12 Oct 2021 19:00:49 GMT  
		Size: 9.3 MB (9343819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e659684a04aace7b984a69bccde2a720cb53304f8905d65b9068605177b2a4b6`  
		Last Modified: Wed, 13 Oct 2021 15:33:06 GMT  
		Size: 16.2 MB (16161376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc86d346babddcb58c40b9188fc289d120a16518eed1782662459497e55f179`  
		Last Modified: Wed, 13 Oct 2021 15:32:54 GMT  
		Size: 2.9 KB (2905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ab61c37e049992dec37a6aba62a2046c0218ac8e88f196d8f297335e469910`  
		Last Modified: Wed, 13 Oct 2021 15:34:22 GMT  
		Size: 32.4 MB (32417295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7392c9c96023c85c1c1c8747fddf4b44295a00702e98de30a55891277c55c92`  
		Last Modified: Wed, 13 Oct 2021 15:33:59 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.20.2` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:124443ca528ab9e7f9f5f300500ea5b8d98c755c4fe8478a1b577852868ed9ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115377157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb9a2610badae699324accc3e50e52294a936812017ad668eba96b450ae0d06a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:28 GMT
ADD file:aed1709ccba6a81b9726b228fad7b81bcf4c16bafe723981ad37076322d78986 in / 
# Tue, 12 Oct 2021 01:41:29 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:59:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:59:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 11:51:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 11:51:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 16 Oct 2021 11:51:35 GMT
ENV TELEGRAF_VERSION=1.20.2
# Sat, 16 Oct 2021 11:51:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sat, 16 Oct 2021 11:51:45 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 16 Oct 2021 11:51:46 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Sat, 16 Oct 2021 11:51:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Oct 2021 11:51:47 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:2ff6d7a9e7d73e4a01b9417518d18c001728c45fa8109ed8f55aaa50e7981482`  
		Last Modified: Tue, 12 Oct 2021 01:48:38 GMT  
		Size: 49.2 MB (49222756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7324ea4098419bc5fa2ac5a138522230bf12cef3996d1740dd00f9d4737d004`  
		Last Modified: Sat, 16 Oct 2021 03:15:37 GMT  
		Size: 7.7 MB (7695063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e213c33a07316d84d829be685bd3b02e1e2bc135f7748c932050e6ed6a3a0d3`  
		Last Modified: Sat, 16 Oct 2021 03:15:37 GMT  
		Size: 9.8 MB (9767289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195fcb7c5d1eb571a72b8f9d97c3baa030a716aa837f3e8228435b153a518cca`  
		Last Modified: Sat, 16 Oct 2021 11:52:14 GMT  
		Size: 17.1 MB (17058985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb3a6b78fdf159f9ca6b70db784a6eafd05eb4f5f46555df56c6d48d032c608`  
		Last Modified: Sat, 16 Oct 2021 11:52:11 GMT  
		Size: 2.9 KB (2879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523dbbcea8d35ab6f724f5585dbbd270602fb850af02b87b2227b77c5bc6ec4d`  
		Last Modified: Sat, 16 Oct 2021 11:52:47 GMT  
		Size: 31.6 MB (31629999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f604607ffed6f61d8be9837a6e259de4749b98d9a2f384a1c16889e5f320e024`  
		Last Modified: Sat, 16 Oct 2021 11:52:42 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.20.2-alpine`

```console
$ docker pull telegraf@sha256:a5fac131412fe7078fb4b7d6d8c4edc5016c984c69cbf1ee787ff59ed5d896c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.20.2-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:884120aaa5b052fcb8727d4def67519b2bb9f697ae20efec50097721abb4a5dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40758696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:135f23862b5d9b6b00e3540179e34be36eb001c54cb5344ed55554a7d73802f7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 20 Sep 2021 22:24:35 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Fri, 08 Oct 2021 17:31:44 GMT
ENV TELEGRAF_VERSION=1.20.2
# Fri, 08 Oct 2021 17:31:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 08 Oct 2021 17:31:56 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 08 Oct 2021 17:31:56 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Fri, 08 Oct 2021 17:31:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Oct 2021 17:31:56 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758daa9673013581700790c0ac7a9855a70445ef1c41bfc2d0ab94288ab13a6b`  
		Last Modified: Mon, 20 Sep 2021 22:25:51 GMT  
		Size: 3.3 MB (3348558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eafdaa25d6c53cc5132e20cbe015727e3bb384607caf6c76ca71f527bfba272`  
		Last Modified: Fri, 08 Oct 2021 17:32:44 GMT  
		Size: 34.6 MB (34595357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d9340b120badda5a4cd2792ac218ece7061af283ead0fbbd6ca756da19a8c2`  
		Last Modified: Fri, 08 Oct 2021 17:32:38 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:a5fac131412fe7078fb4b7d6d8c4edc5016c984c69cbf1ee787ff59ed5d896c5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:884120aaa5b052fcb8727d4def67519b2bb9f697ae20efec50097721abb4a5dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40758696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:135f23862b5d9b6b00e3540179e34be36eb001c54cb5344ed55554a7d73802f7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 20 Sep 2021 22:24:35 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata &&     update-ca-certificates
# Fri, 08 Oct 2021 17:31:44 GMT
ENV TELEGRAF_VERSION=1.20.2
# Fri, 08 Oct 2021 17:31:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Fri, 08 Oct 2021 17:31:56 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 08 Oct 2021 17:31:56 GMT
COPY file:a8a66b0d8dac2aee66897c63ce9b7a3d282bb5d7b796ffb12c2cd9227fed341b in /entrypoint.sh 
# Fri, 08 Oct 2021 17:31:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 08 Oct 2021 17:31:56 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:758daa9673013581700790c0ac7a9855a70445ef1c41bfc2d0ab94288ab13a6b`  
		Last Modified: Mon, 20 Sep 2021 22:25:51 GMT  
		Size: 3.3 MB (3348558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eafdaa25d6c53cc5132e20cbe015727e3bb384607caf6c76ca71f527bfba272`  
		Last Modified: Fri, 08 Oct 2021 17:32:44 GMT  
		Size: 34.6 MB (34595357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2d9340b120badda5a4cd2792ac218ece7061af283ead0fbbd6ca756da19a8c2`  
		Last Modified: Fri, 08 Oct 2021 17:32:38 GMT  
		Size: 182.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:700b5b8fcb46844a7396265d90f0274ceb2e169a9c354b5629a9f235993bb139
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:d7de36f6c04825144b45189eba7c0b363ecb08e63a3a7c8572d8dcf1b4eca73d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120438552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e36bdd348ca3bd084087c93bbb35ece214e69dcd1e17d86389e9a9950e6ba4c2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:53 GMT
ADD file:98c256057b79b141aea9a806a4538cf6c3f340d7e3b0d6e8c363699333f3406b in / 
# Tue, 12 Oct 2021 01:20:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:44:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:44:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Oct 2021 10:25:38 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 10:25:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 13 Oct 2021 10:26:24 GMT
ENV TELEGRAF_VERSION=1.20.2
# Wed, 13 Oct 2021 10:26:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 13 Oct 2021 10:26:28 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 13 Oct 2021 10:26:29 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 13 Oct 2021 10:26:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 10:26:29 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:07471e81507f7cf1100827f10c60c3c0422d1222430e34e527d97ec72b14a193`  
		Last Modified: Tue, 12 Oct 2021 01:26:26 GMT  
		Size: 50.4 MB (50436692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cef1aa2170c001b320769bf8b018ed82d2c94a673e3010ea1ffe152e107419`  
		Last Modified: Tue, 12 Oct 2021 15:54:16 GMT  
		Size: 7.8 MB (7833862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a51f13be8e69cfc526b671d0bbf621b985b0932acd1523050e2995777b5926`  
		Last Modified: Tue, 12 Oct 2021 15:54:17 GMT  
		Size: 10.0 MB (9997204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c91a466291d423e3faad6a8be6ae82e4a4d0550acb67989ac71c98f900e74d41`  
		Last Modified: Wed, 13 Oct 2021 10:26:55 GMT  
		Size: 17.4 MB (17415387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77934da0dce5bef46b239a3871787c2962a08cf1c8b1e629282f0c617b46426`  
		Last Modified: Wed, 13 Oct 2021 10:26:52 GMT  
		Size: 2.9 KB (2906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fe40b78b74cb29485f43d826630febe77421a130fc3a60e984efee2d0cacca`  
		Last Modified: Wed, 13 Oct 2021 10:27:32 GMT  
		Size: 34.8 MB (34752317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b39af786583bce9560759a1517b19efa4b4d9a1a5a9f2613af7358365db368`  
		Last Modified: Wed, 13 Oct 2021 10:27:26 GMT  
		Size: 184.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:1095e724ff8b62ca04c45c86c617eb7fda3a1949be4a31a97f3a3d6871b5695d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (110968719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6367f3beba90bfac51b16bf4bd246bf3117f537226d643b0ee0267b158a791eb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:29:06 GMT
ADD file:b1857dc4fe4fbc4af220829cc6af7169c4555d3f63a3a304db6fa0146b1d5539 in / 
# Tue, 12 Oct 2021 01:29:08 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:39:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:39:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 Oct 2021 15:31:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Wed, 13 Oct 2021 15:31:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 13 Oct 2021 15:31:57 GMT
ENV TELEGRAF_VERSION=1.20.2
# Wed, 13 Oct 2021 15:32:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 13 Oct 2021 15:32:09 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 13 Oct 2021 15:32:10 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Wed, 13 Oct 2021 15:32:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 13 Oct 2021 15:32:11 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:139a906e9407e96c50669130c30fe8fba2681b14aa838a3e52f8753b566ef1c8`  
		Last Modified: Tue, 12 Oct 2021 01:45:13 GMT  
		Size: 45.9 MB (45917899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3907051e2154d5bd4ad15141b8938bc09674039787512494a99b93fd4ebc088d`  
		Last Modified: Tue, 12 Oct 2021 19:00:49 GMT  
		Size: 7.1 MB (7125242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8651d4793d5f4d465002213d2d462c964aaf8665a87d5f9cc0de7384f10eeb10`  
		Last Modified: Tue, 12 Oct 2021 19:00:49 GMT  
		Size: 9.3 MB (9343819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e659684a04aace7b984a69bccde2a720cb53304f8905d65b9068605177b2a4b6`  
		Last Modified: Wed, 13 Oct 2021 15:33:06 GMT  
		Size: 16.2 MB (16161376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc86d346babddcb58c40b9188fc289d120a16518eed1782662459497e55f179`  
		Last Modified: Wed, 13 Oct 2021 15:32:54 GMT  
		Size: 2.9 KB (2905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ab61c37e049992dec37a6aba62a2046c0218ac8e88f196d8f297335e469910`  
		Last Modified: Wed, 13 Oct 2021 15:34:22 GMT  
		Size: 32.4 MB (32417295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7392c9c96023c85c1c1c8747fddf4b44295a00702e98de30a55891277c55c92`  
		Last Modified: Wed, 13 Oct 2021 15:33:59 GMT  
		Size: 183.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:124443ca528ab9e7f9f5f300500ea5b8d98c755c4fe8478a1b577852868ed9ec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115377157 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb9a2610badae699324accc3e50e52294a936812017ad668eba96b450ae0d06a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:28 GMT
ADD file:aed1709ccba6a81b9726b228fad7b81bcf4c16bafe723981ad37076322d78986 in / 
# Tue, 12 Oct 2021 01:41:29 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:59:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:59:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 16 Oct 2021 11:51:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors &&     rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 11:51:08 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Sat, 16 Oct 2021 11:51:35 GMT
ENV TELEGRAF_VERSION=1.20.2
# Sat, 16 Oct 2021 11:51:44 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Sat, 16 Oct 2021 11:51:45 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 16 Oct 2021 11:51:46 GMT
COPY file:7e725b38b34580a28d521266535fcafc651af09f8af8fc6e03ef74768e1b69a2 in /entrypoint.sh 
# Sat, 16 Oct 2021 11:51:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Oct 2021 11:51:47 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:2ff6d7a9e7d73e4a01b9417518d18c001728c45fa8109ed8f55aaa50e7981482`  
		Last Modified: Tue, 12 Oct 2021 01:48:38 GMT  
		Size: 49.2 MB (49222756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7324ea4098419bc5fa2ac5a138522230bf12cef3996d1740dd00f9d4737d004`  
		Last Modified: Sat, 16 Oct 2021 03:15:37 GMT  
		Size: 7.7 MB (7695063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e213c33a07316d84d829be685bd3b02e1e2bc135f7748c932050e6ed6a3a0d3`  
		Last Modified: Sat, 16 Oct 2021 03:15:37 GMT  
		Size: 9.8 MB (9767289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195fcb7c5d1eb571a72b8f9d97c3baa030a716aa837f3e8228435b153a518cca`  
		Last Modified: Sat, 16 Oct 2021 11:52:14 GMT  
		Size: 17.1 MB (17058985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb3a6b78fdf159f9ca6b70db784a6eafd05eb4f5f46555df56c6d48d032c608`  
		Last Modified: Sat, 16 Oct 2021 11:52:11 GMT  
		Size: 2.9 KB (2879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523dbbcea8d35ab6f724f5585dbbd270602fb850af02b87b2227b77c5bc6ec4d`  
		Last Modified: Sat, 16 Oct 2021 11:52:47 GMT  
		Size: 31.6 MB (31629999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f604607ffed6f61d8be9837a6e259de4749b98d9a2f384a1c16889e5f320e024`  
		Last Modified: Sat, 16 Oct 2021 11:52:42 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
