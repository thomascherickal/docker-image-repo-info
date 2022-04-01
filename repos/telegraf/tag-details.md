<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `telegraf`

-	[`telegraf:1.20`](#telegraf120)
-	[`telegraf:1.20-alpine`](#telegraf120-alpine)
-	[`telegraf:1.20.4`](#telegraf1204)
-	[`telegraf:1.20.4-alpine`](#telegraf1204-alpine)
-	[`telegraf:1.21`](#telegraf121)
-	[`telegraf:1.21-alpine`](#telegraf121-alpine)
-	[`telegraf:1.21.4`](#telegraf1214)
-	[`telegraf:1.21.4-alpine`](#telegraf1214-alpine)
-	[`telegraf:1.22`](#telegraf122)
-	[`telegraf:1.22-alpine`](#telegraf122-alpine)
-	[`telegraf:1.22.0`](#telegraf1220)
-	[`telegraf:1.22.0-alpine`](#telegraf1220-alpine)
-	[`telegraf:alpine`](#telegrafalpine)
-	[`telegraf:latest`](#telegraflatest)

## `telegraf:1.20`

```console
$ docker pull telegraf@sha256:3d8c7b1055131318adb575fe314d6461409334b16490eee44fff7bdb6e9ff45c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.20` - linux; amd64

```console
$ docker pull telegraf@sha256:bc92da9a9780c996c6af7065b806498e7a5573512fe7826d0b4238c0a25a7611
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125360077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:443b13b895b975c6e1b47908bf5c7a28195aa1fe6248091b7b593ba8289a94e7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:07 GMT
ADD file:e8d512b08fe2ddc6f2c85831c73e4c72b9c850fa428913d19da4bb1a34f84cf2 in / 
# Tue, 29 Mar 2022 00:22:08 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:29:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:29:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 31 Mar 2022 01:07:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 01:07:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 31 Mar 2022 01:07:14 GMT
ENV TELEGRAF_VERSION=1.20.4
# Thu, 31 Mar 2022 01:07:17 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 31 Mar 2022 01:07:18 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 31 Mar 2022 01:07:18 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 31 Mar 2022 01:07:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 31 Mar 2022 01:07:18 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:dbba69284b2786013fe94fefe0c2e66a7d3cecbb20f6d691d71dac891ee37be5`  
		Last Modified: Tue, 29 Mar 2022 00:26:47 GMT  
		Size: 54.9 MB (54937710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9baf437a1badb6aad2dae5f2cd4a7b53a6c7ab6c14cba1ed1ecb42b4822b0e87`  
		Last Modified: Tue, 29 Mar 2022 17:38:08 GMT  
		Size: 5.2 MB (5155705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ade5c59e324bd7cf369c72ad781c23d37e8fb48c9bbb4abbecafafd9be4cc35`  
		Last Modified: Tue, 29 Mar 2022 17:38:08 GMT  
		Size: 10.9 MB (10874957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0680c11313d76d20633a102c6fc665961c9980b9ecd297f17faf934ec5857281`  
		Last Modified: Thu, 31 Mar 2022 01:08:01 GMT  
		Size: 18.8 MB (18760136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f43e04d38451e900ebbdf9d41cd22c6433e09055242093664915f81b411fcf`  
		Last Modified: Thu, 31 Mar 2022 01:07:57 GMT  
		Size: 2.9 KB (2900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d0da5de3977023965774ff018455933b3316122534d0de9b68db704093b05`  
		Last Modified: Thu, 31 Mar 2022 01:08:04 GMT  
		Size: 35.6 MB (35628327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8aafac2c310c11de722c4ae90aa11c8a70ef2c9fe49025c1b98f23eb1ebcf5`  
		Last Modified: Thu, 31 Mar 2022 01:07:57 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.20` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:82dab9fcb4e6d8a06eec6f01797784e4dfa2aad98623a94a9fcb9689ccf631bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115831796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007e81b085374f8728b08ea407eb6c5fdc3cf0f3be4015bb6da2c81c492d4b1e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 02:17:58 GMT
ADD file:d8d3280d101d611090968c237af923598174e090c533c24bcee805d174e4a6f5 in / 
# Tue, 29 Mar 2022 02:17:59 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 20:06:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 20:06:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Apr 2022 01:33:23 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Apr 2022 01:33:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 01 Apr 2022 01:33:26 GMT
ENV TELEGRAF_VERSION=1.20.4
# Fri, 01 Apr 2022 01:33:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 01 Apr 2022 01:33:38 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Apr 2022 01:33:39 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 01 Apr 2022 01:33:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Apr 2022 01:33:40 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:fc87a15f2d540adb88546a549e56aa0a378d5719bbfd07399e467a095e27d5df`  
		Last Modified: Tue, 29 Mar 2022 02:33:28 GMT  
		Size: 50.1 MB (50133868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7991e015792e592929b68328873d303aff48f6941208e2954283895889e665b3`  
		Last Modified: Wed, 30 Mar 2022 20:30:28 GMT  
		Size: 4.9 MB (4924893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4aa6896142430c96d4b31e28c4d0e3c383d9ae671ce052f26fc7cf68189c058`  
		Last Modified: Wed, 30 Mar 2022 20:30:30 GMT  
		Size: 10.2 MB (10217881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44e9e10874218753b33c76d93ab63fcf6c0c7b13070898eaf005cdf13228180`  
		Last Modified: Fri, 01 Apr 2022 01:35:26 GMT  
		Size: 17.5 MB (17462337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547efda312530826eab241fb2b7aff4b8a1d622fee3c2acac2cf2e17abaaecae`  
		Last Modified: Fri, 01 Apr 2022 01:35:14 GMT  
		Size: 2.9 KB (2898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19219a4a9b534369c00cf5c453bc8e4a02467739b923aea802e58507fd520976`  
		Last Modified: Fri, 01 Apr 2022 01:35:38 GMT  
		Size: 33.1 MB (33089574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8ebfaa21d638157edb0d41011b1768e79f5f6bd09bb2c21c21fbf5a39a637d`  
		Last Modified: Fri, 01 Apr 2022 01:35:14 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.20` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:a2201cc8407df605f1f139d992aec0573ef021fc8333111de31911fa3c663408
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (119979502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9d2dccc88ca18913d5ea3ce917ca581186ea37db4c2b2f79d99cd1a4c724495`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:01 GMT
ADD file:5e8f8c10da6d37a727fb5e1ed13b3dd78769f0ca7e91f0c3510e2edd25177117 in / 
# Tue, 29 Mar 2022 00:43:03 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:13:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:13:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 23:18:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 23:18:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 30 Mar 2022 23:18:57 GMT
ENV TELEGRAF_VERSION=1.20.4
# Wed, 30 Mar 2022 23:19:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 30 Mar 2022 23:19:03 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 30 Mar 2022 23:19:04 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 30 Mar 2022 23:19:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 30 Mar 2022 23:19:05 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:fa223d8c149d7beec8e997e1415ee4961473cafaf88a932f70baf3da56f2c564`  
		Last Modified: Tue, 29 Mar 2022 00:49:33 GMT  
		Size: 53.6 MB (53633710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ffbd2ab15985c19f9e1e3199cdce06090266d20d11dbd3d55fba45de2fcc27`  
		Last Modified: Wed, 30 Mar 2022 02:24:13 GMT  
		Size: 4.9 MB (4938638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3953e76cee2ab175d909ccec1a3399912a690ad621ae88cff787d98419b97bb`  
		Last Modified: Wed, 30 Mar 2022 02:24:14 GMT  
		Size: 10.7 MB (10656993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a939508bbfeff08431d12b3d89969385801628a957c0a7d2b6fa2b55d54025a`  
		Last Modified: Wed, 30 Mar 2022 23:20:02 GMT  
		Size: 18.4 MB (18382668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699770afbd04634c5c13054a9ea8927682515ddfaf2a80cc4f91345063910d0c`  
		Last Modified: Wed, 30 Mar 2022 23:19:59 GMT  
		Size: 2.9 KB (2870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295a48c17eb5e516d444c27597737dc15e4b217597a3cac97257f0ce5577a067`  
		Last Modified: Wed, 30 Mar 2022 23:20:04 GMT  
		Size: 32.4 MB (32364279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82f915cd46bce4cf1d6696d71d45bb64edc7b50221a205b012d29a7eb6631de`  
		Last Modified: Wed, 30 Mar 2022 23:19:59 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.20-alpine`

```console
$ docker pull telegraf@sha256:18208f04e4264f29fdde21513cb8af7699f46269dc85f9e3c8251ca97e5cdfd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.20-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:ae87af551c209e747a1d428e52b01934247e33361205768a44b5cbf45a99131c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41657477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae34594b410235a8b575dcd1f62d236dfcb3013b20c9c3bbdd9d4b14c6c8b1b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:41:23 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 29 Mar 2022 11:41:27 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 29 Mar 2022 11:41:27 GMT
ENV TELEGRAF_VERSION=1.20.4
# Tue, 29 Mar 2022 11:41:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 29 Mar 2022 11:41:33 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 29 Mar 2022 11:41:33 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 29 Mar 2022 11:41:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 11:41:33 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12483063889258e1624f2cfda2d69b39ab8e53e59e8a8648b21b8f38ffdf68c`  
		Last Modified: Tue, 29 Mar 2022 11:42:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8715b1decb53b75ed57959d95918685b6619ce300cd348468d5b68a955744332`  
		Last Modified: Tue, 29 Mar 2022 11:42:15 GMT  
		Size: 3.4 MB (3372370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c302b91722b1494c814231d481f6c1fef691c867bc4ddac9cf48f93543ffc208`  
		Last Modified: Tue, 29 Mar 2022 11:42:21 GMT  
		Size: 35.5 MB (35470116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7286767723515e17c27828b69fd26ee6e8b4361668c533638fb03da8a6a7fb`  
		Last Modified: Tue, 29 Mar 2022 11:42:15 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.20.4`

```console
$ docker pull telegraf@sha256:3d8c7b1055131318adb575fe314d6461409334b16490eee44fff7bdb6e9ff45c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.20.4` - linux; amd64

```console
$ docker pull telegraf@sha256:bc92da9a9780c996c6af7065b806498e7a5573512fe7826d0b4238c0a25a7611
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125360077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:443b13b895b975c6e1b47908bf5c7a28195aa1fe6248091b7b593ba8289a94e7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:07 GMT
ADD file:e8d512b08fe2ddc6f2c85831c73e4c72b9c850fa428913d19da4bb1a34f84cf2 in / 
# Tue, 29 Mar 2022 00:22:08 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:29:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:29:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 31 Mar 2022 01:07:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 01:07:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 31 Mar 2022 01:07:14 GMT
ENV TELEGRAF_VERSION=1.20.4
# Thu, 31 Mar 2022 01:07:17 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 31 Mar 2022 01:07:18 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 31 Mar 2022 01:07:18 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 31 Mar 2022 01:07:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 31 Mar 2022 01:07:18 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:dbba69284b2786013fe94fefe0c2e66a7d3cecbb20f6d691d71dac891ee37be5`  
		Last Modified: Tue, 29 Mar 2022 00:26:47 GMT  
		Size: 54.9 MB (54937710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9baf437a1badb6aad2dae5f2cd4a7b53a6c7ab6c14cba1ed1ecb42b4822b0e87`  
		Last Modified: Tue, 29 Mar 2022 17:38:08 GMT  
		Size: 5.2 MB (5155705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ade5c59e324bd7cf369c72ad781c23d37e8fb48c9bbb4abbecafafd9be4cc35`  
		Last Modified: Tue, 29 Mar 2022 17:38:08 GMT  
		Size: 10.9 MB (10874957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0680c11313d76d20633a102c6fc665961c9980b9ecd297f17faf934ec5857281`  
		Last Modified: Thu, 31 Mar 2022 01:08:01 GMT  
		Size: 18.8 MB (18760136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f43e04d38451e900ebbdf9d41cd22c6433e09055242093664915f81b411fcf`  
		Last Modified: Thu, 31 Mar 2022 01:07:57 GMT  
		Size: 2.9 KB (2900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3d0da5de3977023965774ff018455933b3316122534d0de9b68db704093b05`  
		Last Modified: Thu, 31 Mar 2022 01:08:04 GMT  
		Size: 35.6 MB (35628327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8aafac2c310c11de722c4ae90aa11c8a70ef2c9fe49025c1b98f23eb1ebcf5`  
		Last Modified: Thu, 31 Mar 2022 01:07:57 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.20.4` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:82dab9fcb4e6d8a06eec6f01797784e4dfa2aad98623a94a9fcb9689ccf631bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.8 MB (115831796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007e81b085374f8728b08ea407eb6c5fdc3cf0f3be4015bb6da2c81c492d4b1e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 02:17:58 GMT
ADD file:d8d3280d101d611090968c237af923598174e090c533c24bcee805d174e4a6f5 in / 
# Tue, 29 Mar 2022 02:17:59 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 20:06:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 20:06:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Apr 2022 01:33:23 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Apr 2022 01:33:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 01 Apr 2022 01:33:26 GMT
ENV TELEGRAF_VERSION=1.20.4
# Fri, 01 Apr 2022 01:33:38 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 01 Apr 2022 01:33:38 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Apr 2022 01:33:39 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 01 Apr 2022 01:33:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Apr 2022 01:33:40 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:fc87a15f2d540adb88546a549e56aa0a378d5719bbfd07399e467a095e27d5df`  
		Last Modified: Tue, 29 Mar 2022 02:33:28 GMT  
		Size: 50.1 MB (50133868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7991e015792e592929b68328873d303aff48f6941208e2954283895889e665b3`  
		Last Modified: Wed, 30 Mar 2022 20:30:28 GMT  
		Size: 4.9 MB (4924893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4aa6896142430c96d4b31e28c4d0e3c383d9ae671ce052f26fc7cf68189c058`  
		Last Modified: Wed, 30 Mar 2022 20:30:30 GMT  
		Size: 10.2 MB (10217881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44e9e10874218753b33c76d93ab63fcf6c0c7b13070898eaf005cdf13228180`  
		Last Modified: Fri, 01 Apr 2022 01:35:26 GMT  
		Size: 17.5 MB (17462337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547efda312530826eab241fb2b7aff4b8a1d622fee3c2acac2cf2e17abaaecae`  
		Last Modified: Fri, 01 Apr 2022 01:35:14 GMT  
		Size: 2.9 KB (2898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19219a4a9b534369c00cf5c453bc8e4a02467739b923aea802e58507fd520976`  
		Last Modified: Fri, 01 Apr 2022 01:35:38 GMT  
		Size: 33.1 MB (33089574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8ebfaa21d638157edb0d41011b1768e79f5f6bd09bb2c21c21fbf5a39a637d`  
		Last Modified: Fri, 01 Apr 2022 01:35:14 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.20.4` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:a2201cc8407df605f1f139d992aec0573ef021fc8333111de31911fa3c663408
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (119979502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9d2dccc88ca18913d5ea3ce917ca581186ea37db4c2b2f79d99cd1a4c724495`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:01 GMT
ADD file:5e8f8c10da6d37a727fb5e1ed13b3dd78769f0ca7e91f0c3510e2edd25177117 in / 
# Tue, 29 Mar 2022 00:43:03 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:13:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:13:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 23:18:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 23:18:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 30 Mar 2022 23:18:57 GMT
ENV TELEGRAF_VERSION=1.20.4
# Wed, 30 Mar 2022 23:19:02 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 30 Mar 2022 23:19:03 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 30 Mar 2022 23:19:04 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 30 Mar 2022 23:19:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 30 Mar 2022 23:19:05 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:fa223d8c149d7beec8e997e1415ee4961473cafaf88a932f70baf3da56f2c564`  
		Last Modified: Tue, 29 Mar 2022 00:49:33 GMT  
		Size: 53.6 MB (53633710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ffbd2ab15985c19f9e1e3199cdce06090266d20d11dbd3d55fba45de2fcc27`  
		Last Modified: Wed, 30 Mar 2022 02:24:13 GMT  
		Size: 4.9 MB (4938638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3953e76cee2ab175d909ccec1a3399912a690ad621ae88cff787d98419b97bb`  
		Last Modified: Wed, 30 Mar 2022 02:24:14 GMT  
		Size: 10.7 MB (10656993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a939508bbfeff08431d12b3d89969385801628a957c0a7d2b6fa2b55d54025a`  
		Last Modified: Wed, 30 Mar 2022 23:20:02 GMT  
		Size: 18.4 MB (18382668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699770afbd04634c5c13054a9ea8927682515ddfaf2a80cc4f91345063910d0c`  
		Last Modified: Wed, 30 Mar 2022 23:19:59 GMT  
		Size: 2.9 KB (2870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295a48c17eb5e516d444c27597737dc15e4b217597a3cac97257f0ce5577a067`  
		Last Modified: Wed, 30 Mar 2022 23:20:04 GMT  
		Size: 32.4 MB (32364279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e82f915cd46bce4cf1d6696d71d45bb64edc7b50221a205b012d29a7eb6631de`  
		Last Modified: Wed, 30 Mar 2022 23:19:59 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.20.4-alpine`

```console
$ docker pull telegraf@sha256:18208f04e4264f29fdde21513cb8af7699f46269dc85f9e3c8251ca97e5cdfd1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.20.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:ae87af551c209e747a1d428e52b01934247e33361205768a44b5cbf45a99131c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.7 MB (41657477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae34594b410235a8b575dcd1f62d236dfcb3013b20c9c3bbdd9d4b14c6c8b1b9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:41:23 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 29 Mar 2022 11:41:27 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 29 Mar 2022 11:41:27 GMT
ENV TELEGRAF_VERSION=1.20.4
# Tue, 29 Mar 2022 11:41:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 29 Mar 2022 11:41:33 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 29 Mar 2022 11:41:33 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 29 Mar 2022 11:41:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 11:41:33 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12483063889258e1624f2cfda2d69b39ab8e53e59e8a8648b21b8f38ffdf68c`  
		Last Modified: Tue, 29 Mar 2022 11:42:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8715b1decb53b75ed57959d95918685b6619ce300cd348468d5b68a955744332`  
		Last Modified: Tue, 29 Mar 2022 11:42:15 GMT  
		Size: 3.4 MB (3372370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c302b91722b1494c814231d481f6c1fef691c867bc4ddac9cf48f93543ffc208`  
		Last Modified: Tue, 29 Mar 2022 11:42:21 GMT  
		Size: 35.5 MB (35470116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7286767723515e17c27828b69fd26ee6e8b4361668c533638fb03da8a6a7fb`  
		Last Modified: Tue, 29 Mar 2022 11:42:15 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.21`

```console
$ docker pull telegraf@sha256:bf09772c80bef95d6fb414b0a458d048d23f29baeb67a7225d9d42165eef898b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.21` - linux; amd64

```console
$ docker pull telegraf@sha256:b2bb9a86814df01a23024fb7c20dc0ce5d06aec5bac2c22af5a5550db97a4a84
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127388905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5283e95d06265ae2b147c86f0fa9419ef6f070a86e13474d2e38d075c503578`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:07 GMT
ADD file:e8d512b08fe2ddc6f2c85831c73e4c72b9c850fa428913d19da4bb1a34f84cf2 in / 
# Tue, 29 Mar 2022 00:22:08 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:29:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:29:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 31 Mar 2022 01:07:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 01:07:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 31 Mar 2022 01:07:23 GMT
ENV TELEGRAF_VERSION=1.21.4
# Thu, 31 Mar 2022 01:07:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 31 Mar 2022 01:07:27 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 31 Mar 2022 01:07:27 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 31 Mar 2022 01:07:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 31 Mar 2022 01:07:28 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:dbba69284b2786013fe94fefe0c2e66a7d3cecbb20f6d691d71dac891ee37be5`  
		Last Modified: Tue, 29 Mar 2022 00:26:47 GMT  
		Size: 54.9 MB (54937710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9baf437a1badb6aad2dae5f2cd4a7b53a6c7ab6c14cba1ed1ecb42b4822b0e87`  
		Last Modified: Tue, 29 Mar 2022 17:38:08 GMT  
		Size: 5.2 MB (5155705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ade5c59e324bd7cf369c72ad781c23d37e8fb48c9bbb4abbecafafd9be4cc35`  
		Last Modified: Tue, 29 Mar 2022 17:38:08 GMT  
		Size: 10.9 MB (10874957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0680c11313d76d20633a102c6fc665961c9980b9ecd297f17faf934ec5857281`  
		Last Modified: Thu, 31 Mar 2022 01:08:01 GMT  
		Size: 18.8 MB (18760136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f43e04d38451e900ebbdf9d41cd22c6433e09055242093664915f81b411fcf`  
		Last Modified: Thu, 31 Mar 2022 01:07:57 GMT  
		Size: 2.9 KB (2900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92dad4d5f966cd07ce2cd810ee77da88f90b7f16432a411464dabe4b55ce9af7`  
		Last Modified: Thu, 31 Mar 2022 01:08:21 GMT  
		Size: 37.7 MB (37657153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e087ae8693712659db3c3dfddff07ad2285db4de4da8d90edcfc1efbb239113`  
		Last Modified: Thu, 31 Mar 2022 01:08:14 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.21` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:438223079074a73d323da24c6893d6c9f2e0fb58dcdcae2267e8ebec423e87e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117672928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8557c27edfefa1168fba24e9ad5853ba865c3beac216faca0e15ae439dbc4e41`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 02:17:58 GMT
ADD file:d8d3280d101d611090968c237af923598174e090c533c24bcee805d174e4a6f5 in / 
# Tue, 29 Mar 2022 02:17:59 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 20:06:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 20:06:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Apr 2022 01:33:23 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Apr 2022 01:33:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 01 Apr 2022 01:33:51 GMT
ENV TELEGRAF_VERSION=1.21.4
# Fri, 01 Apr 2022 01:34:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 01 Apr 2022 01:34:04 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Apr 2022 01:34:05 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 01 Apr 2022 01:34:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Apr 2022 01:34:05 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:fc87a15f2d540adb88546a549e56aa0a378d5719bbfd07399e467a095e27d5df`  
		Last Modified: Tue, 29 Mar 2022 02:33:28 GMT  
		Size: 50.1 MB (50133868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7991e015792e592929b68328873d303aff48f6941208e2954283895889e665b3`  
		Last Modified: Wed, 30 Mar 2022 20:30:28 GMT  
		Size: 4.9 MB (4924893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4aa6896142430c96d4b31e28c4d0e3c383d9ae671ce052f26fc7cf68189c058`  
		Last Modified: Wed, 30 Mar 2022 20:30:30 GMT  
		Size: 10.2 MB (10217881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44e9e10874218753b33c76d93ab63fcf6c0c7b13070898eaf005cdf13228180`  
		Last Modified: Fri, 01 Apr 2022 01:35:26 GMT  
		Size: 17.5 MB (17462337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547efda312530826eab241fb2b7aff4b8a1d622fee3c2acac2cf2e17abaaecae`  
		Last Modified: Fri, 01 Apr 2022 01:35:14 GMT  
		Size: 2.9 KB (2898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613ef0264e0c7c195bf8b26068648fa5ce34b55eee59c70d5e6b8920e8a3a01e`  
		Last Modified: Fri, 01 Apr 2022 01:36:14 GMT  
		Size: 34.9 MB (34930708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a51808725988f9e900d828de069c16f24bf3084e9d59d41f1dffb6d1dd81172`  
		Last Modified: Fri, 01 Apr 2022 01:35:49 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.21` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:32a81f79ae9e02dde794f3c0af41e124d3eb7e4fe6b383fb666f67cbc87dda28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121775520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b0cecf6e4c84e4b56a7bd1a9f0eba2437951c4ccd80490b566597a7103f0c60`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:01 GMT
ADD file:5e8f8c10da6d37a727fb5e1ed13b3dd78769f0ca7e91f0c3510e2edd25177117 in / 
# Tue, 29 Mar 2022 00:43:03 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:13:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:13:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 23:18:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 23:18:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 30 Mar 2022 23:19:13 GMT
ENV TELEGRAF_VERSION=1.21.4
# Wed, 30 Mar 2022 23:19:18 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 30 Mar 2022 23:19:19 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 30 Mar 2022 23:19:20 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 30 Mar 2022 23:19:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 30 Mar 2022 23:19:21 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:fa223d8c149d7beec8e997e1415ee4961473cafaf88a932f70baf3da56f2c564`  
		Last Modified: Tue, 29 Mar 2022 00:49:33 GMT  
		Size: 53.6 MB (53633710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ffbd2ab15985c19f9e1e3199cdce06090266d20d11dbd3d55fba45de2fcc27`  
		Last Modified: Wed, 30 Mar 2022 02:24:13 GMT  
		Size: 4.9 MB (4938638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3953e76cee2ab175d909ccec1a3399912a690ad621ae88cff787d98419b97bb`  
		Last Modified: Wed, 30 Mar 2022 02:24:14 GMT  
		Size: 10.7 MB (10656993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a939508bbfeff08431d12b3d89969385801628a957c0a7d2b6fa2b55d54025a`  
		Last Modified: Wed, 30 Mar 2022 23:20:02 GMT  
		Size: 18.4 MB (18382668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699770afbd04634c5c13054a9ea8927682515ddfaf2a80cc4f91345063910d0c`  
		Last Modified: Wed, 30 Mar 2022 23:19:59 GMT  
		Size: 2.9 KB (2870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1707a4b728e30560e82aa0cdfa0480e4d5af2e34da2342f588b219c4ff9cde23`  
		Last Modified: Wed, 30 Mar 2022 23:20:21 GMT  
		Size: 34.2 MB (34160297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b08980a3f329f3fbb5dee8beb2cb8be0fa00fa1de3e4d7fa6c88a3fd0a02cf6`  
		Last Modified: Wed, 30 Mar 2022 23:20:15 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.21-alpine`

```console
$ docker pull telegraf@sha256:8b2b6bb784066c67388eb7426a1bdd3e266d627e10080cf7d383746501732fe7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.21-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:ff78ed6c9dcfc2487c10502fa9dfdb944c3bdf5c41cd99cda403bf1d28463a4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43685581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa08f1b05b5fef5d267d25f8de68669037478f00e03eb149032f4969325e081`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:41:23 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 29 Mar 2022 11:41:27 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 29 Mar 2022 11:41:38 GMT
ENV TELEGRAF_VERSION=1.21.4
# Tue, 29 Mar 2022 11:41:44 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 29 Mar 2022 11:41:45 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 29 Mar 2022 11:41:45 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 29 Mar 2022 11:41:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 11:41:45 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12483063889258e1624f2cfda2d69b39ab8e53e59e8a8648b21b8f38ffdf68c`  
		Last Modified: Tue, 29 Mar 2022 11:42:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8715b1decb53b75ed57959d95918685b6619ce300cd348468d5b68a955744332`  
		Last Modified: Tue, 29 Mar 2022 11:42:15 GMT  
		Size: 3.4 MB (3372370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a8ca82c8269e540b5b4194a36c393c4936ae05c0cccfe604eb1a96310d082f`  
		Last Modified: Tue, 29 Mar 2022 11:42:37 GMT  
		Size: 37.5 MB (37498221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8721f5fda7337910595a43cb7e7bf09941677e58fe5195d953014aae0d3a7fe2`  
		Last Modified: Tue, 29 Mar 2022 11:42:31 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.21.4`

```console
$ docker pull telegraf@sha256:bf09772c80bef95d6fb414b0a458d048d23f29baeb67a7225d9d42165eef898b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.21.4` - linux; amd64

```console
$ docker pull telegraf@sha256:b2bb9a86814df01a23024fb7c20dc0ce5d06aec5bac2c22af5a5550db97a4a84
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127388905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5283e95d06265ae2b147c86f0fa9419ef6f070a86e13474d2e38d075c503578`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:07 GMT
ADD file:e8d512b08fe2ddc6f2c85831c73e4c72b9c850fa428913d19da4bb1a34f84cf2 in / 
# Tue, 29 Mar 2022 00:22:08 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:29:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:29:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 31 Mar 2022 01:07:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 01:07:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 31 Mar 2022 01:07:23 GMT
ENV TELEGRAF_VERSION=1.21.4
# Thu, 31 Mar 2022 01:07:27 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 31 Mar 2022 01:07:27 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 31 Mar 2022 01:07:27 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 31 Mar 2022 01:07:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 31 Mar 2022 01:07:28 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:dbba69284b2786013fe94fefe0c2e66a7d3cecbb20f6d691d71dac891ee37be5`  
		Last Modified: Tue, 29 Mar 2022 00:26:47 GMT  
		Size: 54.9 MB (54937710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9baf437a1badb6aad2dae5f2cd4a7b53a6c7ab6c14cba1ed1ecb42b4822b0e87`  
		Last Modified: Tue, 29 Mar 2022 17:38:08 GMT  
		Size: 5.2 MB (5155705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ade5c59e324bd7cf369c72ad781c23d37e8fb48c9bbb4abbecafafd9be4cc35`  
		Last Modified: Tue, 29 Mar 2022 17:38:08 GMT  
		Size: 10.9 MB (10874957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0680c11313d76d20633a102c6fc665961c9980b9ecd297f17faf934ec5857281`  
		Last Modified: Thu, 31 Mar 2022 01:08:01 GMT  
		Size: 18.8 MB (18760136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f43e04d38451e900ebbdf9d41cd22c6433e09055242093664915f81b411fcf`  
		Last Modified: Thu, 31 Mar 2022 01:07:57 GMT  
		Size: 2.9 KB (2900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92dad4d5f966cd07ce2cd810ee77da88f90b7f16432a411464dabe4b55ce9af7`  
		Last Modified: Thu, 31 Mar 2022 01:08:21 GMT  
		Size: 37.7 MB (37657153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e087ae8693712659db3c3dfddff07ad2285db4de4da8d90edcfc1efbb239113`  
		Last Modified: Thu, 31 Mar 2022 01:08:14 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.21.4` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:438223079074a73d323da24c6893d6c9f2e0fb58dcdcae2267e8ebec423e87e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117672928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8557c27edfefa1168fba24e9ad5853ba865c3beac216faca0e15ae439dbc4e41`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 02:17:58 GMT
ADD file:d8d3280d101d611090968c237af923598174e090c533c24bcee805d174e4a6f5 in / 
# Tue, 29 Mar 2022 02:17:59 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 20:06:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 20:06:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Apr 2022 01:33:23 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Apr 2022 01:33:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 01 Apr 2022 01:33:51 GMT
ENV TELEGRAF_VERSION=1.21.4
# Fri, 01 Apr 2022 01:34:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 01 Apr 2022 01:34:04 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Apr 2022 01:34:05 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 01 Apr 2022 01:34:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Apr 2022 01:34:05 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:fc87a15f2d540adb88546a549e56aa0a378d5719bbfd07399e467a095e27d5df`  
		Last Modified: Tue, 29 Mar 2022 02:33:28 GMT  
		Size: 50.1 MB (50133868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7991e015792e592929b68328873d303aff48f6941208e2954283895889e665b3`  
		Last Modified: Wed, 30 Mar 2022 20:30:28 GMT  
		Size: 4.9 MB (4924893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4aa6896142430c96d4b31e28c4d0e3c383d9ae671ce052f26fc7cf68189c058`  
		Last Modified: Wed, 30 Mar 2022 20:30:30 GMT  
		Size: 10.2 MB (10217881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44e9e10874218753b33c76d93ab63fcf6c0c7b13070898eaf005cdf13228180`  
		Last Modified: Fri, 01 Apr 2022 01:35:26 GMT  
		Size: 17.5 MB (17462337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547efda312530826eab241fb2b7aff4b8a1d622fee3c2acac2cf2e17abaaecae`  
		Last Modified: Fri, 01 Apr 2022 01:35:14 GMT  
		Size: 2.9 KB (2898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613ef0264e0c7c195bf8b26068648fa5ce34b55eee59c70d5e6b8920e8a3a01e`  
		Last Modified: Fri, 01 Apr 2022 01:36:14 GMT  
		Size: 34.9 MB (34930708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a51808725988f9e900d828de069c16f24bf3084e9d59d41f1dffb6d1dd81172`  
		Last Modified: Fri, 01 Apr 2022 01:35:49 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.21.4` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:32a81f79ae9e02dde794f3c0af41e124d3eb7e4fe6b383fb666f67cbc87dda28
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.8 MB (121775520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b0cecf6e4c84e4b56a7bd1a9f0eba2437951c4ccd80490b566597a7103f0c60`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:01 GMT
ADD file:5e8f8c10da6d37a727fb5e1ed13b3dd78769f0ca7e91f0c3510e2edd25177117 in / 
# Tue, 29 Mar 2022 00:43:03 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:13:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:13:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 23:18:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 23:18:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 30 Mar 2022 23:19:13 GMT
ENV TELEGRAF_VERSION=1.21.4
# Wed, 30 Mar 2022 23:19:18 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 30 Mar 2022 23:19:19 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 30 Mar 2022 23:19:20 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 30 Mar 2022 23:19:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 30 Mar 2022 23:19:21 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:fa223d8c149d7beec8e997e1415ee4961473cafaf88a932f70baf3da56f2c564`  
		Last Modified: Tue, 29 Mar 2022 00:49:33 GMT  
		Size: 53.6 MB (53633710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ffbd2ab15985c19f9e1e3199cdce06090266d20d11dbd3d55fba45de2fcc27`  
		Last Modified: Wed, 30 Mar 2022 02:24:13 GMT  
		Size: 4.9 MB (4938638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3953e76cee2ab175d909ccec1a3399912a690ad621ae88cff787d98419b97bb`  
		Last Modified: Wed, 30 Mar 2022 02:24:14 GMT  
		Size: 10.7 MB (10656993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a939508bbfeff08431d12b3d89969385801628a957c0a7d2b6fa2b55d54025a`  
		Last Modified: Wed, 30 Mar 2022 23:20:02 GMT  
		Size: 18.4 MB (18382668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699770afbd04634c5c13054a9ea8927682515ddfaf2a80cc4f91345063910d0c`  
		Last Modified: Wed, 30 Mar 2022 23:19:59 GMT  
		Size: 2.9 KB (2870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1707a4b728e30560e82aa0cdfa0480e4d5af2e34da2342f588b219c4ff9cde23`  
		Last Modified: Wed, 30 Mar 2022 23:20:21 GMT  
		Size: 34.2 MB (34160297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b08980a3f329f3fbb5dee8beb2cb8be0fa00fa1de3e4d7fa6c88a3fd0a02cf6`  
		Last Modified: Wed, 30 Mar 2022 23:20:15 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.21.4-alpine`

```console
$ docker pull telegraf@sha256:8b2b6bb784066c67388eb7426a1bdd3e266d627e10080cf7d383746501732fe7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.21.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:ff78ed6c9dcfc2487c10502fa9dfdb944c3bdf5c41cd99cda403bf1d28463a4a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.7 MB (43685581 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa08f1b05b5fef5d267d25f8de68669037478f00e03eb149032f4969325e081`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:41:23 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 29 Mar 2022 11:41:27 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 29 Mar 2022 11:41:38 GMT
ENV TELEGRAF_VERSION=1.21.4
# Tue, 29 Mar 2022 11:41:44 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 29 Mar 2022 11:41:45 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 29 Mar 2022 11:41:45 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 29 Mar 2022 11:41:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 11:41:45 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12483063889258e1624f2cfda2d69b39ab8e53e59e8a8648b21b8f38ffdf68c`  
		Last Modified: Tue, 29 Mar 2022 11:42:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8715b1decb53b75ed57959d95918685b6619ce300cd348468d5b68a955744332`  
		Last Modified: Tue, 29 Mar 2022 11:42:15 GMT  
		Size: 3.4 MB (3372370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65a8ca82c8269e540b5b4194a36c393c4936ae05c0cccfe604eb1a96310d082f`  
		Last Modified: Tue, 29 Mar 2022 11:42:37 GMT  
		Size: 37.5 MB (37498221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8721f5fda7337910595a43cb7e7bf09941677e58fe5195d953014aae0d3a7fe2`  
		Last Modified: Tue, 29 Mar 2022 11:42:31 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.22`

```console
$ docker pull telegraf@sha256:1ff45b21d3e3c2de446ea01f14de3bcfa563e4211e6a7b35292ea89230224242
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.22` - linux; amd64

```console
$ docker pull telegraf@sha256:425d7915e4c0b5c26a3bca98572f898be3cbb626b7e570a08de32ecfa71be5e9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128703039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9e2b2b325832b09aa049eee6f079aa8fc2743b8a54ee5cca9a474fb2687f43a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:07 GMT
ADD file:e8d512b08fe2ddc6f2c85831c73e4c72b9c850fa428913d19da4bb1a34f84cf2 in / 
# Tue, 29 Mar 2022 00:22:08 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:29:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:29:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 31 Mar 2022 01:07:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 01:07:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 31 Mar 2022 01:07:32 GMT
ENV TELEGRAF_VERSION=1.22.0
# Thu, 31 Mar 2022 01:07:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 31 Mar 2022 01:07:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 31 Mar 2022 01:07:36 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 31 Mar 2022 01:07:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 31 Mar 2022 01:07:36 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:dbba69284b2786013fe94fefe0c2e66a7d3cecbb20f6d691d71dac891ee37be5`  
		Last Modified: Tue, 29 Mar 2022 00:26:47 GMT  
		Size: 54.9 MB (54937710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9baf437a1badb6aad2dae5f2cd4a7b53a6c7ab6c14cba1ed1ecb42b4822b0e87`  
		Last Modified: Tue, 29 Mar 2022 17:38:08 GMT  
		Size: 5.2 MB (5155705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ade5c59e324bd7cf369c72ad781c23d37e8fb48c9bbb4abbecafafd9be4cc35`  
		Last Modified: Tue, 29 Mar 2022 17:38:08 GMT  
		Size: 10.9 MB (10874957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0680c11313d76d20633a102c6fc665961c9980b9ecd297f17faf934ec5857281`  
		Last Modified: Thu, 31 Mar 2022 01:08:01 GMT  
		Size: 18.8 MB (18760136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f43e04d38451e900ebbdf9d41cd22c6433e09055242093664915f81b411fcf`  
		Last Modified: Thu, 31 Mar 2022 01:07:57 GMT  
		Size: 2.9 KB (2900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7762e1308d94056cd014dd773e13755505e8f9208653c693464a169541ed3ed7`  
		Last Modified: Thu, 31 Mar 2022 01:08:39 GMT  
		Size: 39.0 MB (38971290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c37f1343ecb3eb111e2d63f49e1521618400013d8f0d644312f394afd5e6ac`  
		Last Modified: Thu, 31 Mar 2022 01:08:32 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.22` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:c682efa2cf4fa51501680b746e1713c8b5db8bfc4ef9277466eb903191c643be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118853629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7966a3bd2c35751c633a732cc60435ef2724553f603017fdb83d0333012392b8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 02:17:58 GMT
ADD file:d8d3280d101d611090968c237af923598174e090c533c24bcee805d174e4a6f5 in / 
# Tue, 29 Mar 2022 02:17:59 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 20:06:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 20:06:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Apr 2022 01:33:23 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Apr 2022 01:33:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 01 Apr 2022 01:34:16 GMT
ENV TELEGRAF_VERSION=1.22.0
# Fri, 01 Apr 2022 01:34:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 01 Apr 2022 01:34:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Apr 2022 01:34:29 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 01 Apr 2022 01:34:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Apr 2022 01:34:30 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:fc87a15f2d540adb88546a549e56aa0a378d5719bbfd07399e467a095e27d5df`  
		Last Modified: Tue, 29 Mar 2022 02:33:28 GMT  
		Size: 50.1 MB (50133868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7991e015792e592929b68328873d303aff48f6941208e2954283895889e665b3`  
		Last Modified: Wed, 30 Mar 2022 20:30:28 GMT  
		Size: 4.9 MB (4924893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4aa6896142430c96d4b31e28c4d0e3c383d9ae671ce052f26fc7cf68189c058`  
		Last Modified: Wed, 30 Mar 2022 20:30:30 GMT  
		Size: 10.2 MB (10217881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44e9e10874218753b33c76d93ab63fcf6c0c7b13070898eaf005cdf13228180`  
		Last Modified: Fri, 01 Apr 2022 01:35:26 GMT  
		Size: 17.5 MB (17462337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547efda312530826eab241fb2b7aff4b8a1d622fee3c2acac2cf2e17abaaecae`  
		Last Modified: Fri, 01 Apr 2022 01:35:14 GMT  
		Size: 2.9 KB (2898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a4e5c15c9c1da9825522e56d650c37a465fa65d3392fb91417589265628fb1`  
		Last Modified: Fri, 01 Apr 2022 01:36:51 GMT  
		Size: 36.1 MB (36111409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be25be2bd652e1422318a69e00931ae94316be5b84fa03cda0b46c55337e35f`  
		Last Modified: Fri, 01 Apr 2022 01:36:26 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.22` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:92b030cbc5b0a84d82c9c058577bae0f7b0295fbaca51af8a2ef112c0385e9f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.9 MB (122899972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c38a08475161948eea1eb79633f4b3d0fe9170fa1433fd56262d9d1b74525d5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:01 GMT
ADD file:5e8f8c10da6d37a727fb5e1ed13b3dd78769f0ca7e91f0c3510e2edd25177117 in / 
# Tue, 29 Mar 2022 00:43:03 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:13:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:13:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 23:18:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 23:18:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 30 Mar 2022 23:19:27 GMT
ENV TELEGRAF_VERSION=1.22.0
# Wed, 30 Mar 2022 23:19:32 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 30 Mar 2022 23:19:33 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 30 Mar 2022 23:19:34 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 30 Mar 2022 23:19:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 30 Mar 2022 23:19:35 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:fa223d8c149d7beec8e997e1415ee4961473cafaf88a932f70baf3da56f2c564`  
		Last Modified: Tue, 29 Mar 2022 00:49:33 GMT  
		Size: 53.6 MB (53633710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ffbd2ab15985c19f9e1e3199cdce06090266d20d11dbd3d55fba45de2fcc27`  
		Last Modified: Wed, 30 Mar 2022 02:24:13 GMT  
		Size: 4.9 MB (4938638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3953e76cee2ab175d909ccec1a3399912a690ad621ae88cff787d98419b97bb`  
		Last Modified: Wed, 30 Mar 2022 02:24:14 GMT  
		Size: 10.7 MB (10656993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a939508bbfeff08431d12b3d89969385801628a957c0a7d2b6fa2b55d54025a`  
		Last Modified: Wed, 30 Mar 2022 23:20:02 GMT  
		Size: 18.4 MB (18382668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699770afbd04634c5c13054a9ea8927682515ddfaf2a80cc4f91345063910d0c`  
		Last Modified: Wed, 30 Mar 2022 23:19:59 GMT  
		Size: 2.9 KB (2870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac24096c1f6cabb104ad4825ad5248bfb39f658b7e398b246732ed29dd94af52`  
		Last Modified: Wed, 30 Mar 2022 23:20:38 GMT  
		Size: 35.3 MB (35284748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84458c7c9459225f2c31cc25fa6b966857e84b7c6b9a92bd25979f996980188`  
		Last Modified: Wed, 30 Mar 2022 23:20:32 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.22-alpine`

```console
$ docker pull telegraf@sha256:424450fdaef91e34e5aaba8747e2ab02efd1f8723c8163f3f7a96f2a91518df2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.22-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:d44e8c87225ae620b614503b0f477f2b54b7aea0a56d8eb1818985a242671bc3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44998913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f1d30ad8eba8b967efb60e073eb530212dcd82379e1ecad34c91b691ad6b346`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:41:23 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 29 Mar 2022 11:41:27 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 29 Mar 2022 11:41:50 GMT
ENV TELEGRAF_VERSION=1.22.0
# Tue, 29 Mar 2022 11:41:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 29 Mar 2022 11:41:55 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 29 Mar 2022 11:41:55 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 29 Mar 2022 11:41:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 11:41:56 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12483063889258e1624f2cfda2d69b39ab8e53e59e8a8648b21b8f38ffdf68c`  
		Last Modified: Tue, 29 Mar 2022 11:42:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8715b1decb53b75ed57959d95918685b6619ce300cd348468d5b68a955744332`  
		Last Modified: Tue, 29 Mar 2022 11:42:15 GMT  
		Size: 3.4 MB (3372370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebd1e86fd79a7ce24a623e29ab82215266c019aac3645257e6820b5de04e15c`  
		Last Modified: Tue, 29 Mar 2022 11:42:54 GMT  
		Size: 38.8 MB (38811554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b760ea9da2751f295a2d903071db891d9e3402f1d618530ccf2f2124c17dcdd`  
		Last Modified: Tue, 29 Mar 2022 11:42:48 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.22.0`

```console
$ docker pull telegraf@sha256:1ff45b21d3e3c2de446ea01f14de3bcfa563e4211e6a7b35292ea89230224242
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.22.0` - linux; amd64

```console
$ docker pull telegraf@sha256:425d7915e4c0b5c26a3bca98572f898be3cbb626b7e570a08de32ecfa71be5e9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128703039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9e2b2b325832b09aa049eee6f079aa8fc2743b8a54ee5cca9a474fb2687f43a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:07 GMT
ADD file:e8d512b08fe2ddc6f2c85831c73e4c72b9c850fa428913d19da4bb1a34f84cf2 in / 
# Tue, 29 Mar 2022 00:22:08 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:29:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:29:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 31 Mar 2022 01:07:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 01:07:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 31 Mar 2022 01:07:32 GMT
ENV TELEGRAF_VERSION=1.22.0
# Thu, 31 Mar 2022 01:07:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 31 Mar 2022 01:07:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 31 Mar 2022 01:07:36 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 31 Mar 2022 01:07:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 31 Mar 2022 01:07:36 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:dbba69284b2786013fe94fefe0c2e66a7d3cecbb20f6d691d71dac891ee37be5`  
		Last Modified: Tue, 29 Mar 2022 00:26:47 GMT  
		Size: 54.9 MB (54937710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9baf437a1badb6aad2dae5f2cd4a7b53a6c7ab6c14cba1ed1ecb42b4822b0e87`  
		Last Modified: Tue, 29 Mar 2022 17:38:08 GMT  
		Size: 5.2 MB (5155705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ade5c59e324bd7cf369c72ad781c23d37e8fb48c9bbb4abbecafafd9be4cc35`  
		Last Modified: Tue, 29 Mar 2022 17:38:08 GMT  
		Size: 10.9 MB (10874957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0680c11313d76d20633a102c6fc665961c9980b9ecd297f17faf934ec5857281`  
		Last Modified: Thu, 31 Mar 2022 01:08:01 GMT  
		Size: 18.8 MB (18760136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f43e04d38451e900ebbdf9d41cd22c6433e09055242093664915f81b411fcf`  
		Last Modified: Thu, 31 Mar 2022 01:07:57 GMT  
		Size: 2.9 KB (2900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7762e1308d94056cd014dd773e13755505e8f9208653c693464a169541ed3ed7`  
		Last Modified: Thu, 31 Mar 2022 01:08:39 GMT  
		Size: 39.0 MB (38971290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c37f1343ecb3eb111e2d63f49e1521618400013d8f0d644312f394afd5e6ac`  
		Last Modified: Thu, 31 Mar 2022 01:08:32 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.22.0` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:c682efa2cf4fa51501680b746e1713c8b5db8bfc4ef9277466eb903191c643be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118853629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7966a3bd2c35751c633a732cc60435ef2724553f603017fdb83d0333012392b8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 02:17:58 GMT
ADD file:d8d3280d101d611090968c237af923598174e090c533c24bcee805d174e4a6f5 in / 
# Tue, 29 Mar 2022 02:17:59 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 20:06:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 20:06:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Apr 2022 01:33:23 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Apr 2022 01:33:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 01 Apr 2022 01:34:16 GMT
ENV TELEGRAF_VERSION=1.22.0
# Fri, 01 Apr 2022 01:34:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 01 Apr 2022 01:34:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Apr 2022 01:34:29 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 01 Apr 2022 01:34:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Apr 2022 01:34:30 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:fc87a15f2d540adb88546a549e56aa0a378d5719bbfd07399e467a095e27d5df`  
		Last Modified: Tue, 29 Mar 2022 02:33:28 GMT  
		Size: 50.1 MB (50133868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7991e015792e592929b68328873d303aff48f6941208e2954283895889e665b3`  
		Last Modified: Wed, 30 Mar 2022 20:30:28 GMT  
		Size: 4.9 MB (4924893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4aa6896142430c96d4b31e28c4d0e3c383d9ae671ce052f26fc7cf68189c058`  
		Last Modified: Wed, 30 Mar 2022 20:30:30 GMT  
		Size: 10.2 MB (10217881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44e9e10874218753b33c76d93ab63fcf6c0c7b13070898eaf005cdf13228180`  
		Last Modified: Fri, 01 Apr 2022 01:35:26 GMT  
		Size: 17.5 MB (17462337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547efda312530826eab241fb2b7aff4b8a1d622fee3c2acac2cf2e17abaaecae`  
		Last Modified: Fri, 01 Apr 2022 01:35:14 GMT  
		Size: 2.9 KB (2898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a4e5c15c9c1da9825522e56d650c37a465fa65d3392fb91417589265628fb1`  
		Last Modified: Fri, 01 Apr 2022 01:36:51 GMT  
		Size: 36.1 MB (36111409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be25be2bd652e1422318a69e00931ae94316be5b84fa03cda0b46c55337e35f`  
		Last Modified: Fri, 01 Apr 2022 01:36:26 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.22.0` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:92b030cbc5b0a84d82c9c058577bae0f7b0295fbaca51af8a2ef112c0385e9f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.9 MB (122899972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c38a08475161948eea1eb79633f4b3d0fe9170fa1433fd56262d9d1b74525d5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:01 GMT
ADD file:5e8f8c10da6d37a727fb5e1ed13b3dd78769f0ca7e91f0c3510e2edd25177117 in / 
# Tue, 29 Mar 2022 00:43:03 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:13:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:13:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 23:18:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 23:18:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 30 Mar 2022 23:19:27 GMT
ENV TELEGRAF_VERSION=1.22.0
# Wed, 30 Mar 2022 23:19:32 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 30 Mar 2022 23:19:33 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 30 Mar 2022 23:19:34 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 30 Mar 2022 23:19:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 30 Mar 2022 23:19:35 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:fa223d8c149d7beec8e997e1415ee4961473cafaf88a932f70baf3da56f2c564`  
		Last Modified: Tue, 29 Mar 2022 00:49:33 GMT  
		Size: 53.6 MB (53633710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ffbd2ab15985c19f9e1e3199cdce06090266d20d11dbd3d55fba45de2fcc27`  
		Last Modified: Wed, 30 Mar 2022 02:24:13 GMT  
		Size: 4.9 MB (4938638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3953e76cee2ab175d909ccec1a3399912a690ad621ae88cff787d98419b97bb`  
		Last Modified: Wed, 30 Mar 2022 02:24:14 GMT  
		Size: 10.7 MB (10656993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a939508bbfeff08431d12b3d89969385801628a957c0a7d2b6fa2b55d54025a`  
		Last Modified: Wed, 30 Mar 2022 23:20:02 GMT  
		Size: 18.4 MB (18382668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699770afbd04634c5c13054a9ea8927682515ddfaf2a80cc4f91345063910d0c`  
		Last Modified: Wed, 30 Mar 2022 23:19:59 GMT  
		Size: 2.9 KB (2870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac24096c1f6cabb104ad4825ad5248bfb39f658b7e398b246732ed29dd94af52`  
		Last Modified: Wed, 30 Mar 2022 23:20:38 GMT  
		Size: 35.3 MB (35284748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84458c7c9459225f2c31cc25fa6b966857e84b7c6b9a92bd25979f996980188`  
		Last Modified: Wed, 30 Mar 2022 23:20:32 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.22.0-alpine`

```console
$ docker pull telegraf@sha256:424450fdaef91e34e5aaba8747e2ab02efd1f8723c8163f3f7a96f2a91518df2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.22.0-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:d44e8c87225ae620b614503b0f477f2b54b7aea0a56d8eb1818985a242671bc3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44998913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f1d30ad8eba8b967efb60e073eb530212dcd82379e1ecad34c91b691ad6b346`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:41:23 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 29 Mar 2022 11:41:27 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 29 Mar 2022 11:41:50 GMT
ENV TELEGRAF_VERSION=1.22.0
# Tue, 29 Mar 2022 11:41:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 29 Mar 2022 11:41:55 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 29 Mar 2022 11:41:55 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 29 Mar 2022 11:41:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 11:41:56 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12483063889258e1624f2cfda2d69b39ab8e53e59e8a8648b21b8f38ffdf68c`  
		Last Modified: Tue, 29 Mar 2022 11:42:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8715b1decb53b75ed57959d95918685b6619ce300cd348468d5b68a955744332`  
		Last Modified: Tue, 29 Mar 2022 11:42:15 GMT  
		Size: 3.4 MB (3372370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebd1e86fd79a7ce24a623e29ab82215266c019aac3645257e6820b5de04e15c`  
		Last Modified: Tue, 29 Mar 2022 11:42:54 GMT  
		Size: 38.8 MB (38811554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b760ea9da2751f295a2d903071db891d9e3402f1d618530ccf2f2124c17dcdd`  
		Last Modified: Tue, 29 Mar 2022 11:42:48 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:424450fdaef91e34e5aaba8747e2ab02efd1f8723c8163f3f7a96f2a91518df2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:d44e8c87225ae620b614503b0f477f2b54b7aea0a56d8eb1818985a242671bc3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.0 MB (44998913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f1d30ad8eba8b967efb60e073eb530212dcd82379e1ecad34c91b691ad6b346`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:36 GMT
ADD file:3b5a33c96fd3c10d0c438d907ce172903f7b2bde0f4e5107831e135ddf111b19 in / 
# Tue, 29 Mar 2022 00:19:36 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 11:41:23 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Tue, 29 Mar 2022 11:41:27 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Tue, 29 Mar 2022 11:41:50 GMT
ENV TELEGRAF_VERSION=1.22.0
# Tue, 29 Mar 2022 11:41:55 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 29 Mar 2022 11:41:55 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 29 Mar 2022 11:41:55 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 29 Mar 2022 11:41:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 29 Mar 2022 11:41:56 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:40e059520d199e1a1a259089077f2a0c879951c9a4540490bad3a0d7714c6ae7`  
		Last Modified: Mon, 28 Mar 2022 23:30:57 GMT  
		Size: 2.8 MB (2814512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12483063889258e1624f2cfda2d69b39ab8e53e59e8a8648b21b8f38ffdf68c`  
		Last Modified: Tue, 29 Mar 2022 11:42:15 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8715b1decb53b75ed57959d95918685b6619ce300cd348468d5b68a955744332`  
		Last Modified: Tue, 29 Mar 2022 11:42:15 GMT  
		Size: 3.4 MB (3372370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebd1e86fd79a7ce24a623e29ab82215266c019aac3645257e6820b5de04e15c`  
		Last Modified: Tue, 29 Mar 2022 11:42:54 GMT  
		Size: 38.8 MB (38811554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b760ea9da2751f295a2d903071db891d9e3402f1d618530ccf2f2124c17dcdd`  
		Last Modified: Tue, 29 Mar 2022 11:42:48 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:1ff45b21d3e3c2de446ea01f14de3bcfa563e4211e6a7b35292ea89230224242
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:425d7915e4c0b5c26a3bca98572f898be3cbb626b7e570a08de32ecfa71be5e9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128703039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9e2b2b325832b09aa049eee6f079aa8fc2743b8a54ee5cca9a474fb2687f43a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:07 GMT
ADD file:e8d512b08fe2ddc6f2c85831c73e4c72b9c850fa428913d19da4bb1a34f84cf2 in / 
# Tue, 29 Mar 2022 00:22:08 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:29:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:29:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 31 Mar 2022 01:07:12 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 31 Mar 2022 01:07:14 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 31 Mar 2022 01:07:32 GMT
ENV TELEGRAF_VERSION=1.22.0
# Thu, 31 Mar 2022 01:07:35 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 31 Mar 2022 01:07:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 31 Mar 2022 01:07:36 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 31 Mar 2022 01:07:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 31 Mar 2022 01:07:36 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:dbba69284b2786013fe94fefe0c2e66a7d3cecbb20f6d691d71dac891ee37be5`  
		Last Modified: Tue, 29 Mar 2022 00:26:47 GMT  
		Size: 54.9 MB (54937710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9baf437a1badb6aad2dae5f2cd4a7b53a6c7ab6c14cba1ed1ecb42b4822b0e87`  
		Last Modified: Tue, 29 Mar 2022 17:38:08 GMT  
		Size: 5.2 MB (5155705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ade5c59e324bd7cf369c72ad781c23d37e8fb48c9bbb4abbecafafd9be4cc35`  
		Last Modified: Tue, 29 Mar 2022 17:38:08 GMT  
		Size: 10.9 MB (10874957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0680c11313d76d20633a102c6fc665961c9980b9ecd297f17faf934ec5857281`  
		Last Modified: Thu, 31 Mar 2022 01:08:01 GMT  
		Size: 18.8 MB (18760136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80f43e04d38451e900ebbdf9d41cd22c6433e09055242093664915f81b411fcf`  
		Last Modified: Thu, 31 Mar 2022 01:07:57 GMT  
		Size: 2.9 KB (2900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7762e1308d94056cd014dd773e13755505e8f9208653c693464a169541ed3ed7`  
		Last Modified: Thu, 31 Mar 2022 01:08:39 GMT  
		Size: 39.0 MB (38971290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c37f1343ecb3eb111e2d63f49e1521618400013d8f0d644312f394afd5e6ac`  
		Last Modified: Thu, 31 Mar 2022 01:08:32 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:c682efa2cf4fa51501680b746e1713c8b5db8bfc4ef9277466eb903191c643be
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118853629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7966a3bd2c35751c633a732cc60435ef2724553f603017fdb83d0333012392b8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 02:17:58 GMT
ADD file:d8d3280d101d611090968c237af923598174e090c533c24bcee805d174e4a6f5 in / 
# Tue, 29 Mar 2022 02:17:59 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 20:06:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 20:06:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Apr 2022 01:33:23 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Fri, 01 Apr 2022 01:33:25 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Fri, 01 Apr 2022 01:34:16 GMT
ENV TELEGRAF_VERSION=1.22.0
# Fri, 01 Apr 2022 01:34:28 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Fri, 01 Apr 2022 01:34:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Apr 2022 01:34:29 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Fri, 01 Apr 2022 01:34:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Apr 2022 01:34:30 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:fc87a15f2d540adb88546a549e56aa0a378d5719bbfd07399e467a095e27d5df`  
		Last Modified: Tue, 29 Mar 2022 02:33:28 GMT  
		Size: 50.1 MB (50133868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7991e015792e592929b68328873d303aff48f6941208e2954283895889e665b3`  
		Last Modified: Wed, 30 Mar 2022 20:30:28 GMT  
		Size: 4.9 MB (4924893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4aa6896142430c96d4b31e28c4d0e3c383d9ae671ce052f26fc7cf68189c058`  
		Last Modified: Wed, 30 Mar 2022 20:30:30 GMT  
		Size: 10.2 MB (10217881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b44e9e10874218753b33c76d93ab63fcf6c0c7b13070898eaf005cdf13228180`  
		Last Modified: Fri, 01 Apr 2022 01:35:26 GMT  
		Size: 17.5 MB (17462337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547efda312530826eab241fb2b7aff4b8a1d622fee3c2acac2cf2e17abaaecae`  
		Last Modified: Fri, 01 Apr 2022 01:35:14 GMT  
		Size: 2.9 KB (2898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a4e5c15c9c1da9825522e56d650c37a465fa65d3392fb91417589265628fb1`  
		Last Modified: Fri, 01 Apr 2022 01:36:51 GMT  
		Size: 36.1 MB (36111409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be25be2bd652e1422318a69e00931ae94316be5b84fa03cda0b46c55337e35f`  
		Last Modified: Fri, 01 Apr 2022 01:36:26 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:92b030cbc5b0a84d82c9c058577bae0f7b0295fbaca51af8a2ef112c0385e9f5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.9 MB (122899972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c38a08475161948eea1eb79633f4b3d0fe9170fa1433fd56262d9d1b74525d5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:01 GMT
ADD file:5e8f8c10da6d37a727fb5e1ed13b3dd78769f0ca7e91f0c3510e2edd25177117 in / 
# Tue, 29 Mar 2022 00:43:03 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:13:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:13:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 23:18:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 23:18:56 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 30 Mar 2022 23:19:27 GMT
ENV TELEGRAF_VERSION=1.22.0
# Wed, 30 Mar 2022 23:19:32 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 30 Mar 2022 23:19:33 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 30 Mar 2022 23:19:34 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 30 Mar 2022 23:19:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 30 Mar 2022 23:19:35 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:fa223d8c149d7beec8e997e1415ee4961473cafaf88a932f70baf3da56f2c564`  
		Last Modified: Tue, 29 Mar 2022 00:49:33 GMT  
		Size: 53.6 MB (53633710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ffbd2ab15985c19f9e1e3199cdce06090266d20d11dbd3d55fba45de2fcc27`  
		Last Modified: Wed, 30 Mar 2022 02:24:13 GMT  
		Size: 4.9 MB (4938638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3953e76cee2ab175d909ccec1a3399912a690ad621ae88cff787d98419b97bb`  
		Last Modified: Wed, 30 Mar 2022 02:24:14 GMT  
		Size: 10.7 MB (10656993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a939508bbfeff08431d12b3d89969385801628a957c0a7d2b6fa2b55d54025a`  
		Last Modified: Wed, 30 Mar 2022 23:20:02 GMT  
		Size: 18.4 MB (18382668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699770afbd04634c5c13054a9ea8927682515ddfaf2a80cc4f91345063910d0c`  
		Last Modified: Wed, 30 Mar 2022 23:19:59 GMT  
		Size: 2.9 KB (2870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac24096c1f6cabb104ad4825ad5248bfb39f658b7e398b246732ed29dd94af52`  
		Last Modified: Wed, 30 Mar 2022 23:20:38 GMT  
		Size: 35.3 MB (35284748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e84458c7c9459225f2c31cc25fa6b966857e84b7c6b9a92bd25979f996980188`  
		Last Modified: Wed, 30 Mar 2022 23:20:32 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
