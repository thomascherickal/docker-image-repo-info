<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `telegraf`

-	[`telegraf:1.24`](#telegraf124)
-	[`telegraf:1.24-alpine`](#telegraf124-alpine)
-	[`telegraf:1.24.4`](#telegraf1244)
-	[`telegraf:1.24.4-alpine`](#telegraf1244-alpine)
-	[`telegraf:1.25`](#telegraf125)
-	[`telegraf:1.25-alpine`](#telegraf125-alpine)
-	[`telegraf:1.25.3`](#telegraf1253)
-	[`telegraf:1.25.3-alpine`](#telegraf1253-alpine)
-	[`telegraf:1.26`](#telegraf126)
-	[`telegraf:1.26-alpine`](#telegraf126-alpine)
-	[`telegraf:1.26.0`](#telegraf1260)
-	[`telegraf:1.26.0-alpine`](#telegraf1260-alpine)
-	[`telegraf:alpine`](#telegrafalpine)
-	[`telegraf:latest`](#telegraflatest)

## `telegraf:1.24`

```console
$ docker pull telegraf@sha256:dc48cee4eb5aa3cb8036bfd9ea4039351e013d66278fd4629e3f8b6d4f1f6a5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.24` - linux; amd64

```console
$ docker pull telegraf@sha256:9f0f2c43458e8e5f253c45b939abc7ab452b9f9b5f2bf1cf97cc157123ddeab1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134318806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71635c24badddbdf4e0a7ef22563ac1ea23bb19c8ab49069b29f7ac9365f6eab`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 22:44:56 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 22:44:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Mar 2023 22:45:10 GMT
ENV TELEGRAF_VERSION=1.24.4
# Wed, 01 Mar 2023 22:45:13 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 01 Mar 2023 22:45:13 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 01 Mar 2023 22:45:13 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 01 Mar 2023 22:45:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Mar 2023 22:45:14 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf193c1022e32f7a3ffb7be36f631ad081fb01f134f9b6b7b2affb285555deaf`  
		Last Modified: Wed, 01 Mar 2023 22:45:46 GMT  
		Size: 18.8 MB (18760000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c9df80cc94227316d89c5f6e893978f283e80e43d1e9ef432d0f63e9d55fbd`  
		Last Modified: Wed, 01 Mar 2023 22:45:42 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d4204e219e4fd734daa90188b50ab2a721f63de0f492434e40c3048f556e5f`  
		Last Modified: Wed, 01 Mar 2023 22:46:05 GMT  
		Size: 44.5 MB (44467427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f26a6982af674187778b63594b334dc86f083c0c8953582529ce8ac1f502383`  
		Last Modified: Wed, 01 Mar 2023 22:45:58 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.24` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:fb6a8679d4e25fa0de1eaebde69906c80f30cf53488e82ab285b5906447876cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124335708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecd19f94898823b2e8467ef893a5dba86e1015513b7a393579a40a4821e51707`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:45 GMT
ADD file:95a5e178e353a9a46c230d78b0ef83309dd487651c34e47e972ed3dae08ea00b in / 
# Wed, 01 Mar 2023 01:57:45 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:32:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:11:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:11:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 02 Mar 2023 02:12:05 GMT
ENV TELEGRAF_VERSION=1.24.4
# Thu, 02 Mar 2023 02:12:10 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 02 Mar 2023 02:12:10 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 02 Mar 2023 02:12:10 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 02 Mar 2023 02:12:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Mar 2023 02:12:11 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:30bee4bd8986478b5a9ecaaaba83525049f0b9b5a63ca88de878568bb6b83292`  
		Last Modified: Wed, 01 Mar 2023 02:02:32 GMT  
		Size: 50.2 MB (50212046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c2a83a9963df1d0618a3bef56d5f278e39b96940e18347e3575f30d199fb89`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 4.9 MB (4934569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6953f57698d5630bc57919975af4718f7e2eae8d6489d17ceab15dd2ab6e6`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 10.2 MB (10217796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11573ebb43311f57cffeeec94ddd828520b1890e520cdf00a9f48ba4e26fc3e6`  
		Last Modified: Thu, 02 Mar 2023 02:12:47 GMT  
		Size: 17.5 MB (17462043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ccafa66610ea2f48523ec2e133f7674459cc603987fa085111e952ed756e36`  
		Last Modified: Thu, 02 Mar 2023 02:12:44 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2b30889c1110f17a935c64c7cf0cc7985e1958baf503905dcb46473ef804ad`  
		Last Modified: Thu, 02 Mar 2023 02:13:08 GMT  
		Size: 41.5 MB (41507105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcc155d57d92b0e89d1f1505c0ce8b777c9d0971c5fcdb933e496dde923322b`  
		Last Modified: Thu, 02 Mar 2023 02:13:01 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.24` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:65960aef38e4a3e9cbb3fca388c7205633fdda4226263566b2ffa561cdb7d8c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128635563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df9ba9191050ac131ea608cd47d776def87baaaaf6ede6f694e193dfc5406b2a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:49:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 17:23:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:23:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Mar 2023 17:23:13 GMT
ENV TELEGRAF_VERSION=1.24.4
# Wed, 01 Mar 2023 17:23:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 01 Mar 2023 17:23:17 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 01 Mar 2023 17:23:17 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 01 Mar 2023 17:23:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Mar 2023 17:23:17 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8a090f23f28b92f40160bc1a686e3bd5cd4bbd00713a7133631cb2189575f2`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 5.2 MB (5152682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec29ff8525a3f037f4cc74d2925846a9a8c985469b4ae98fa34099110288987c`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 10.9 MB (10873588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22eb8d3d8ab6628e804f35dc6d9ebb9f557fe977afd366b59909f5114fd4c6ff`  
		Last Modified: Wed, 01 Mar 2023 17:23:38 GMT  
		Size: 18.6 MB (18598416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d38dd1a04d89bbeb2779d4abf2e671d1f39492b3df3b607f0115d47e7944b8f`  
		Last Modified: Wed, 01 Mar 2023 17:23:35 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf4e0434760dce92262e17b8b3d0b78855fdab59f021a940f13f4465288309b`  
		Last Modified: Wed, 01 Mar 2023 17:23:54 GMT  
		Size: 40.3 MB (40305514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739e829021f255d00752a89a1ff9b2885b663b6e0c361b42d173d8611dde8997`  
		Last Modified: Wed, 01 Mar 2023 17:23:48 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.24-alpine`

```console
$ docker pull telegraf@sha256:60731c36742033a7e74d95b4bdf127c385a159bc9def6fd8e04499daedfe8c24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.24-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:4f9aef3ed5f8359716aabc50590220ef0f61e49894e5ea0aafd00d3a8c422793
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50340866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1e96b4f3558bc6b945ee49d52d467ed79d92afa3694245420ae39363cdb9c06`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 13 Mar 2023 23:20:26 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 13 Mar 2023 23:20:26 GMT
ENV TELEGRAF_VERSION=1.24.4
# Mon, 13 Mar 2023 23:20:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 13 Mar 2023 23:20:32 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 13 Mar 2023 23:20:33 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 13 Mar 2023 23:20:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Mar 2023 23:20:33 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd826afb15e0fb2da9a39fa76ad385840640783fb85064837ac42d7088a83f5b`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 2.7 MB (2671874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0acf5bcd75b999381ca4bc011fb9d2e12f8e048263b76d936ba944c6d54a59`  
		Last Modified: Mon, 13 Mar 2023 23:21:25 GMT  
		Size: 44.3 MB (44293940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb0c7893d80cddabfa4e1c16a5d284780201b4a9af6dc49502f69e45cce8c6`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.24.4`

```console
$ docker pull telegraf@sha256:dc48cee4eb5aa3cb8036bfd9ea4039351e013d66278fd4629e3f8b6d4f1f6a5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.24.4` - linux; amd64

```console
$ docker pull telegraf@sha256:9f0f2c43458e8e5f253c45b939abc7ab452b9f9b5f2bf1cf97cc157123ddeab1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134318806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71635c24badddbdf4e0a7ef22563ac1ea23bb19c8ab49069b29f7ac9365f6eab`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 22:44:56 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 22:44:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Mar 2023 22:45:10 GMT
ENV TELEGRAF_VERSION=1.24.4
# Wed, 01 Mar 2023 22:45:13 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 01 Mar 2023 22:45:13 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 01 Mar 2023 22:45:13 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 01 Mar 2023 22:45:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Mar 2023 22:45:14 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf193c1022e32f7a3ffb7be36f631ad081fb01f134f9b6b7b2affb285555deaf`  
		Last Modified: Wed, 01 Mar 2023 22:45:46 GMT  
		Size: 18.8 MB (18760000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c9df80cc94227316d89c5f6e893978f283e80e43d1e9ef432d0f63e9d55fbd`  
		Last Modified: Wed, 01 Mar 2023 22:45:42 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60d4204e219e4fd734daa90188b50ab2a721f63de0f492434e40c3048f556e5f`  
		Last Modified: Wed, 01 Mar 2023 22:46:05 GMT  
		Size: 44.5 MB (44467427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f26a6982af674187778b63594b334dc86f083c0c8953582529ce8ac1f502383`  
		Last Modified: Wed, 01 Mar 2023 22:45:58 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.24.4` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:fb6a8679d4e25fa0de1eaebde69906c80f30cf53488e82ab285b5906447876cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.3 MB (124335708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecd19f94898823b2e8467ef893a5dba86e1015513b7a393579a40a4821e51707`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:45 GMT
ADD file:95a5e178e353a9a46c230d78b0ef83309dd487651c34e47e972ed3dae08ea00b in / 
# Wed, 01 Mar 2023 01:57:45 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:32:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:11:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:11:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 02 Mar 2023 02:12:05 GMT
ENV TELEGRAF_VERSION=1.24.4
# Thu, 02 Mar 2023 02:12:10 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 02 Mar 2023 02:12:10 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 02 Mar 2023 02:12:10 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 02 Mar 2023 02:12:11 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Mar 2023 02:12:11 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:30bee4bd8986478b5a9ecaaaba83525049f0b9b5a63ca88de878568bb6b83292`  
		Last Modified: Wed, 01 Mar 2023 02:02:32 GMT  
		Size: 50.2 MB (50212046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c2a83a9963df1d0618a3bef56d5f278e39b96940e18347e3575f30d199fb89`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 4.9 MB (4934569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6953f57698d5630bc57919975af4718f7e2eae8d6489d17ceab15dd2ab6e6`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 10.2 MB (10217796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11573ebb43311f57cffeeec94ddd828520b1890e520cdf00a9f48ba4e26fc3e6`  
		Last Modified: Thu, 02 Mar 2023 02:12:47 GMT  
		Size: 17.5 MB (17462043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ccafa66610ea2f48523ec2e133f7674459cc603987fa085111e952ed756e36`  
		Last Modified: Thu, 02 Mar 2023 02:12:44 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e2b30889c1110f17a935c64c7cf0cc7985e1958baf503905dcb46473ef804ad`  
		Last Modified: Thu, 02 Mar 2023 02:13:08 GMT  
		Size: 41.5 MB (41507105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffcc155d57d92b0e89d1f1505c0ce8b777c9d0971c5fcdb933e496dde923322b`  
		Last Modified: Thu, 02 Mar 2023 02:13:01 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.24.4` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:65960aef38e4a3e9cbb3fca388c7205633fdda4226263566b2ffa561cdb7d8c2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.6 MB (128635563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df9ba9191050ac131ea608cd47d776def87baaaaf6ede6f694e193dfc5406b2a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:49:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 17:23:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:23:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Mar 2023 17:23:13 GMT
ENV TELEGRAF_VERSION=1.24.4
# Wed, 01 Mar 2023 17:23:16 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 01 Mar 2023 17:23:17 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 01 Mar 2023 17:23:17 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 01 Mar 2023 17:23:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Mar 2023 17:23:17 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8a090f23f28b92f40160bc1a686e3bd5cd4bbd00713a7133631cb2189575f2`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 5.2 MB (5152682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec29ff8525a3f037f4cc74d2925846a9a8c985469b4ae98fa34099110288987c`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 10.9 MB (10873588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22eb8d3d8ab6628e804f35dc6d9ebb9f557fe977afd366b59909f5114fd4c6ff`  
		Last Modified: Wed, 01 Mar 2023 17:23:38 GMT  
		Size: 18.6 MB (18598416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d38dd1a04d89bbeb2779d4abf2e671d1f39492b3df3b607f0115d47e7944b8f`  
		Last Modified: Wed, 01 Mar 2023 17:23:35 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf4e0434760dce92262e17b8b3d0b78855fdab59f021a940f13f4465288309b`  
		Last Modified: Wed, 01 Mar 2023 17:23:54 GMT  
		Size: 40.3 MB (40305514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739e829021f255d00752a89a1ff9b2885b663b6e0c361b42d173d8611dde8997`  
		Last Modified: Wed, 01 Mar 2023 17:23:48 GMT  
		Size: 339.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.24.4-alpine`

```console
$ docker pull telegraf@sha256:60731c36742033a7e74d95b4bdf127c385a159bc9def6fd8e04499daedfe8c24
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.24.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:4f9aef3ed5f8359716aabc50590220ef0f61e49894e5ea0aafd00d3a8c422793
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50340866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1e96b4f3558bc6b945ee49d52d467ed79d92afa3694245420ae39363cdb9c06`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 13 Mar 2023 23:20:26 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 13 Mar 2023 23:20:26 GMT
ENV TELEGRAF_VERSION=1.24.4
# Mon, 13 Mar 2023 23:20:32 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 13 Mar 2023 23:20:32 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 13 Mar 2023 23:20:33 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 13 Mar 2023 23:20:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Mar 2023 23:20:33 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd826afb15e0fb2da9a39fa76ad385840640783fb85064837ac42d7088a83f5b`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 2.7 MB (2671874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0acf5bcd75b999381ca4bc011fb9d2e12f8e048263b76d936ba944c6d54a59`  
		Last Modified: Mon, 13 Mar 2023 23:21:25 GMT  
		Size: 44.3 MB (44293940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bb0c7893d80cddabfa4e1c16a5d284780201b4a9af6dc49502f69e45cce8c6`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25`

```console
$ docker pull telegraf@sha256:c0ea630ccdce911024440adc04b252ed31c305dcc39e79e73d4da7c5e7d5950a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.25` - linux; amd64

```console
$ docker pull telegraf@sha256:169f87fb5de800f2233bcd599d52d6df371a1702c19b390d2a31a8ff2495a8fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.4 MB (136428019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:679c6522f7ad7e915087406fdfef60113a390765f6680ed424c8a980dea5227f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 22:44:56 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 22:44:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Mar 2023 22:45:18 GMT
ENV TELEGRAF_VERSION=1.25.3
# Wed, 01 Mar 2023 22:45:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 01 Mar 2023 22:45:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 01 Mar 2023 22:45:22 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 01 Mar 2023 22:45:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Mar 2023 22:45:22 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf193c1022e32f7a3ffb7be36f631ad081fb01f134f9b6b7b2affb285555deaf`  
		Last Modified: Wed, 01 Mar 2023 22:45:46 GMT  
		Size: 18.8 MB (18760000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c9df80cc94227316d89c5f6e893978f283e80e43d1e9ef432d0f63e9d55fbd`  
		Last Modified: Wed, 01 Mar 2023 22:45:42 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e102c98e5bfa3905b5ebcef1e5040aa2236b84cc69d2f6bcccde52335889b0`  
		Last Modified: Wed, 01 Mar 2023 22:46:22 GMT  
		Size: 46.6 MB (46576643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f21ac248cd64058c00328c508b7ad0e449505e08c1e030d419d05e3b18a66ba`  
		Last Modified: Wed, 01 Mar 2023 22:46:14 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:0e46b28d0969858f83c6a1c2234c9330d8b9d72f3f175a5c4181e27a524d1638
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126212576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6d4dc592b221ed3fd3cd8fad9bffa8bdf950a3a89d4510d574c536d29e97e14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:45 GMT
ADD file:95a5e178e353a9a46c230d78b0ef83309dd487651c34e47e972ed3dae08ea00b in / 
# Wed, 01 Mar 2023 01:57:45 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:32:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:11:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:11:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 02 Mar 2023 02:12:15 GMT
ENV TELEGRAF_VERSION=1.25.3
# Thu, 02 Mar 2023 02:12:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 02 Mar 2023 02:12:21 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 02 Mar 2023 02:12:21 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 02 Mar 2023 02:12:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Mar 2023 02:12:21 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:30bee4bd8986478b5a9ecaaaba83525049f0b9b5a63ca88de878568bb6b83292`  
		Last Modified: Wed, 01 Mar 2023 02:02:32 GMT  
		Size: 50.2 MB (50212046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c2a83a9963df1d0618a3bef56d5f278e39b96940e18347e3575f30d199fb89`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 4.9 MB (4934569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6953f57698d5630bc57919975af4718f7e2eae8d6489d17ceab15dd2ab6e6`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 10.2 MB (10217796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11573ebb43311f57cffeeec94ddd828520b1890e520cdf00a9f48ba4e26fc3e6`  
		Last Modified: Thu, 02 Mar 2023 02:12:47 GMT  
		Size: 17.5 MB (17462043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ccafa66610ea2f48523ec2e133f7674459cc603987fa085111e952ed756e36`  
		Last Modified: Thu, 02 Mar 2023 02:12:44 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc87c725f1d75a4f5ebb8fb81c6a8d4f7fec87adcca998a4ee375cbee933ac73`  
		Last Modified: Thu, 02 Mar 2023 02:13:26 GMT  
		Size: 43.4 MB (43383972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785cd9a6cdcd8a908f77aad2e0cb15102af862a54d52067811de681bad2eed12`  
		Last Modified: Thu, 02 Mar 2023 02:13:18 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:ca3d688e2b22166c0a76ba376545eed9aa124addcc2f59c7539081fea2397866
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130645260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:624d13df0d985eaeb8d9e8794c5fbfa04160c73c7e03d1f34a3603374cae17ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:49:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 17:23:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:23:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Mar 2023 17:23:19 GMT
ENV TELEGRAF_VERSION=1.25.3
# Wed, 01 Mar 2023 17:23:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 01 Mar 2023 17:23:23 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 01 Mar 2023 17:23:23 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 01 Mar 2023 17:23:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Mar 2023 17:23:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8a090f23f28b92f40160bc1a686e3bd5cd4bbd00713a7133631cb2189575f2`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 5.2 MB (5152682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec29ff8525a3f037f4cc74d2925846a9a8c985469b4ae98fa34099110288987c`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 10.9 MB (10873588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22eb8d3d8ab6628e804f35dc6d9ebb9f557fe977afd366b59909f5114fd4c6ff`  
		Last Modified: Wed, 01 Mar 2023 17:23:38 GMT  
		Size: 18.6 MB (18598416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d38dd1a04d89bbeb2779d4abf2e671d1f39492b3df3b607f0115d47e7944b8f`  
		Last Modified: Wed, 01 Mar 2023 17:23:35 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2427f4d0777d36eab42907bfe01bd6970181194d601214218a73fba5c6b1a83d`  
		Last Modified: Wed, 01 Mar 2023 17:24:07 GMT  
		Size: 42.3 MB (42315206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e60fa91e6535fcdb67e38bbdb4adbccdaa28b4b4a109aad5f8e719a4222bc47`  
		Last Modified: Wed, 01 Mar 2023 17:24:02 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25-alpine`

```console
$ docker pull telegraf@sha256:c1d4cd6d19f7e5dbbdccf2b9a7abdc9425bc5af7c648bcf4635dd32a43f2bba9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.25-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:5d730bef2e960d5878ce2d1d8b464f56c8d05c483fbfbfb107d0cab0560a66c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52439637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b61509ba4087676533c03ef935ec49b4139dbd8f4e5d095a569975b2ccd72a9b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 13 Mar 2023 23:20:26 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 13 Mar 2023 23:20:38 GMT
ENV TELEGRAF_VERSION=1.25.3
# Mon, 13 Mar 2023 23:20:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 13 Mar 2023 23:20:43 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 13 Mar 2023 23:20:43 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 13 Mar 2023 23:20:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Mar 2023 23:20:44 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd826afb15e0fb2da9a39fa76ad385840640783fb85064837ac42d7088a83f5b`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 2.7 MB (2671874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbb2532b0ac0aa25d71c5bf7ed2fa82b40c9a5bec95fa3395fe16a657926d586`  
		Last Modified: Mon, 13 Mar 2023 23:21:41 GMT  
		Size: 46.4 MB (46392712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd6fd00f74609d1fa7a2e1c657d902325dcee6bfe0bc2db86625bd0752143bc`  
		Last Modified: Mon, 13 Mar 2023 23:21:33 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25.3`

```console
$ docker pull telegraf@sha256:c0ea630ccdce911024440adc04b252ed31c305dcc39e79e73d4da7c5e7d5950a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.25.3` - linux; amd64

```console
$ docker pull telegraf@sha256:169f87fb5de800f2233bcd599d52d6df371a1702c19b390d2a31a8ff2495a8fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.4 MB (136428019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:679c6522f7ad7e915087406fdfef60113a390765f6680ed424c8a980dea5227f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 22:44:56 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 22:44:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Mar 2023 22:45:18 GMT
ENV TELEGRAF_VERSION=1.25.3
# Wed, 01 Mar 2023 22:45:22 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 01 Mar 2023 22:45:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 01 Mar 2023 22:45:22 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 01 Mar 2023 22:45:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Mar 2023 22:45:22 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf193c1022e32f7a3ffb7be36f631ad081fb01f134f9b6b7b2affb285555deaf`  
		Last Modified: Wed, 01 Mar 2023 22:45:46 GMT  
		Size: 18.8 MB (18760000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c9df80cc94227316d89c5f6e893978f283e80e43d1e9ef432d0f63e9d55fbd`  
		Last Modified: Wed, 01 Mar 2023 22:45:42 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e102c98e5bfa3905b5ebcef1e5040aa2236b84cc69d2f6bcccde52335889b0`  
		Last Modified: Wed, 01 Mar 2023 22:46:22 GMT  
		Size: 46.6 MB (46576643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f21ac248cd64058c00328c508b7ad0e449505e08c1e030d419d05e3b18a66ba`  
		Last Modified: Wed, 01 Mar 2023 22:46:14 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25.3` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:0e46b28d0969858f83c6a1c2234c9330d8b9d72f3f175a5c4181e27a524d1638
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.2 MB (126212576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6d4dc592b221ed3fd3cd8fad9bffa8bdf950a3a89d4510d574c536d29e97e14`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:45 GMT
ADD file:95a5e178e353a9a46c230d78b0ef83309dd487651c34e47e972ed3dae08ea00b in / 
# Wed, 01 Mar 2023 01:57:45 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:32:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:11:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:11:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 02 Mar 2023 02:12:15 GMT
ENV TELEGRAF_VERSION=1.25.3
# Thu, 02 Mar 2023 02:12:21 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 02 Mar 2023 02:12:21 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 02 Mar 2023 02:12:21 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 02 Mar 2023 02:12:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 02 Mar 2023 02:12:21 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:30bee4bd8986478b5a9ecaaaba83525049f0b9b5a63ca88de878568bb6b83292`  
		Last Modified: Wed, 01 Mar 2023 02:02:32 GMT  
		Size: 50.2 MB (50212046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c2a83a9963df1d0618a3bef56d5f278e39b96940e18347e3575f30d199fb89`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 4.9 MB (4934569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6953f57698d5630bc57919975af4718f7e2eae8d6489d17ceab15dd2ab6e6`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 10.2 MB (10217796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11573ebb43311f57cffeeec94ddd828520b1890e520cdf00a9f48ba4e26fc3e6`  
		Last Modified: Thu, 02 Mar 2023 02:12:47 GMT  
		Size: 17.5 MB (17462043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ccafa66610ea2f48523ec2e133f7674459cc603987fa085111e952ed756e36`  
		Last Modified: Thu, 02 Mar 2023 02:12:44 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc87c725f1d75a4f5ebb8fb81c6a8d4f7fec87adcca998a4ee375cbee933ac73`  
		Last Modified: Thu, 02 Mar 2023 02:13:26 GMT  
		Size: 43.4 MB (43383972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785cd9a6cdcd8a908f77aad2e0cb15102af862a54d52067811de681bad2eed12`  
		Last Modified: Thu, 02 Mar 2023 02:13:18 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25.3` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:ca3d688e2b22166c0a76ba376545eed9aa124addcc2f59c7539081fea2397866
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.6 MB (130645260 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:624d13df0d985eaeb8d9e8794c5fbfa04160c73c7e03d1f34a3603374cae17ca`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:49:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 17:23:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:23:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 01 Mar 2023 17:23:19 GMT
ENV TELEGRAF_VERSION=1.25.3
# Wed, 01 Mar 2023 17:23:23 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 01 Mar 2023 17:23:23 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 01 Mar 2023 17:23:23 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 01 Mar 2023 17:23:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Mar 2023 17:23:24 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8a090f23f28b92f40160bc1a686e3bd5cd4bbd00713a7133631cb2189575f2`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 5.2 MB (5152682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec29ff8525a3f037f4cc74d2925846a9a8c985469b4ae98fa34099110288987c`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 10.9 MB (10873588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22eb8d3d8ab6628e804f35dc6d9ebb9f557fe977afd366b59909f5114fd4c6ff`  
		Last Modified: Wed, 01 Mar 2023 17:23:38 GMT  
		Size: 18.6 MB (18598416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d38dd1a04d89bbeb2779d4abf2e671d1f39492b3df3b607f0115d47e7944b8f`  
		Last Modified: Wed, 01 Mar 2023 17:23:35 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2427f4d0777d36eab42907bfe01bd6970181194d601214218a73fba5c6b1a83d`  
		Last Modified: Wed, 01 Mar 2023 17:24:07 GMT  
		Size: 42.3 MB (42315206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e60fa91e6535fcdb67e38bbdb4adbccdaa28b4b4a109aad5f8e719a4222bc47`  
		Last Modified: Wed, 01 Mar 2023 17:24:02 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25.3-alpine`

```console
$ docker pull telegraf@sha256:c1d4cd6d19f7e5dbbdccf2b9a7abdc9425bc5af7c648bcf4635dd32a43f2bba9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.25.3-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:5d730bef2e960d5878ce2d1d8b464f56c8d05c483fbfbfb107d0cab0560a66c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52439637 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b61509ba4087676533c03ef935ec49b4139dbd8f4e5d095a569975b2ccd72a9b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 13 Mar 2023 23:20:26 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 13 Mar 2023 23:20:38 GMT
ENV TELEGRAF_VERSION=1.25.3
# Mon, 13 Mar 2023 23:20:43 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 13 Mar 2023 23:20:43 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 13 Mar 2023 23:20:43 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 13 Mar 2023 23:20:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Mar 2023 23:20:44 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd826afb15e0fb2da9a39fa76ad385840640783fb85064837ac42d7088a83f5b`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 2.7 MB (2671874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbb2532b0ac0aa25d71c5bf7ed2fa82b40c9a5bec95fa3395fe16a657926d586`  
		Last Modified: Mon, 13 Mar 2023 23:21:41 GMT  
		Size: 46.4 MB (46392712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd6fd00f74609d1fa7a2e1c657d902325dcee6bfe0bc2db86625bd0752143bc`  
		Last Modified: Mon, 13 Mar 2023 23:21:33 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26`

```console
$ docker pull telegraf@sha256:9f2974a238166819844013871b97ee75f7faabc802fef526fb2eec10916a7d76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.26` - linux; amd64

```console
$ docker pull telegraf@sha256:b22a40470d623b5acde30b3a4a718023dfe4fb7a4a3b0c467f4c81c4705b4d92
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137754851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2019f20bfaeecc55ae49be297185887713beca56522838df0997cfbdac6bf47f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 22:44:56 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 22:44:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 13 Mar 2023 23:20:46 GMT
ENV TELEGRAF_VERSION=1.26.0
# Mon, 13 Mar 2023 23:20:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Mon, 13 Mar 2023 23:20:50 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 13 Mar 2023 23:20:50 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Mon, 13 Mar 2023 23:20:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Mar 2023 23:20:50 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf193c1022e32f7a3ffb7be36f631ad081fb01f134f9b6b7b2affb285555deaf`  
		Last Modified: Wed, 01 Mar 2023 22:45:46 GMT  
		Size: 18.8 MB (18760000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c9df80cc94227316d89c5f6e893978f283e80e43d1e9ef432d0f63e9d55fbd`  
		Last Modified: Wed, 01 Mar 2023 22:45:42 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673fc4c4ba02a37619a21438cdcdca908b172fc42147868639db45ec3fb6c868`  
		Last Modified: Mon, 13 Mar 2023 23:21:56 GMT  
		Size: 47.9 MB (47903475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9510743483be48ca555a663080f43443280238d2e4f581a05e920f21ba0f6e55`  
		Last Modified: Mon, 13 Mar 2023 23:21:49 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:02d25e290efa3488cb127f5b6f5f91587dbce246da83c7159256388e80d4f25e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127484742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82c0ed710458710f5cc47eb3161f37c690684de0455361eefdfb335c16559dcb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:45 GMT
ADD file:95a5e178e353a9a46c230d78b0ef83309dd487651c34e47e972ed3dae08ea00b in / 
# Wed, 01 Mar 2023 01:57:45 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:32:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:11:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:11:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 13 Mar 2023 23:32:47 GMT
ENV TELEGRAF_VERSION=1.26.0
# Mon, 13 Mar 2023 23:32:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Mon, 13 Mar 2023 23:32:54 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 13 Mar 2023 23:32:54 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Mon, 13 Mar 2023 23:32:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Mar 2023 23:32:54 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:30bee4bd8986478b5a9ecaaaba83525049f0b9b5a63ca88de878568bb6b83292`  
		Last Modified: Wed, 01 Mar 2023 02:02:32 GMT  
		Size: 50.2 MB (50212046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c2a83a9963df1d0618a3bef56d5f278e39b96940e18347e3575f30d199fb89`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 4.9 MB (4934569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6953f57698d5630bc57919975af4718f7e2eae8d6489d17ceab15dd2ab6e6`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 10.2 MB (10217796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11573ebb43311f57cffeeec94ddd828520b1890e520cdf00a9f48ba4e26fc3e6`  
		Last Modified: Thu, 02 Mar 2023 02:12:47 GMT  
		Size: 17.5 MB (17462043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ccafa66610ea2f48523ec2e133f7674459cc603987fa085111e952ed756e36`  
		Last Modified: Thu, 02 Mar 2023 02:12:44 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1446a202e285ef1da1532997410dab2bdd154bb0d0c2eaa1b1e463beaf115f`  
		Last Modified: Mon, 13 Mar 2023 23:33:28 GMT  
		Size: 44.7 MB (44656137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e54a59597676f8d916a5c25c0194baaa1a93172ecc350b71358bf929ed6eef`  
		Last Modified: Mon, 13 Mar 2023 23:33:20 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:3dd788ec2fce2306c7ad33da4bd46d921897e0a038c031e710d70649faaf7e10
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131875171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48735df5b1fe414f8b8133972005360e4e6a9f42c5fb8a514789535110b71a2d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:49:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 17:23:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:23:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 13 Mar 2023 23:47:10 GMT
ENV TELEGRAF_VERSION=1.26.0
# Mon, 13 Mar 2023 23:47:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Mon, 13 Mar 2023 23:47:15 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 13 Mar 2023 23:47:15 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Mon, 13 Mar 2023 23:47:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Mar 2023 23:47:15 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8a090f23f28b92f40160bc1a686e3bd5cd4bbd00713a7133631cb2189575f2`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 5.2 MB (5152682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec29ff8525a3f037f4cc74d2925846a9a8c985469b4ae98fa34099110288987c`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 10.9 MB (10873588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22eb8d3d8ab6628e804f35dc6d9ebb9f557fe977afd366b59909f5114fd4c6ff`  
		Last Modified: Wed, 01 Mar 2023 17:23:38 GMT  
		Size: 18.6 MB (18598416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d38dd1a04d89bbeb2779d4abf2e671d1f39492b3df3b607f0115d47e7944b8f`  
		Last Modified: Wed, 01 Mar 2023 17:23:35 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfffa8c42f969c4305e41af97e9ffc752f1d05e717c90c69e88740f8f0107b24`  
		Last Modified: Mon, 13 Mar 2023 23:47:49 GMT  
		Size: 43.5 MB (43545118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60e9733dd9fb36a4aecc845a26c726b03079e633d5fe0869544476020c4e1fe`  
		Last Modified: Mon, 13 Mar 2023 23:47:44 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26-alpine`

```console
$ docker pull telegraf@sha256:07cde4c35d7b0a68485daae6f2749b7743a26d0ff01128869b9c525cd7026a53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.26-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:f2b25cdbc5059c3dd9c98300621363e5a4baa5c48abdff5efd18446621589ff0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53783007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b56be065cfc49ed415b7ef5b32f186d241c12dbc65da685975abf15445063485`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 13 Mar 2023 23:20:26 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 13 Mar 2023 23:20:53 GMT
ENV TELEGRAF_VERSION=1.26.0
# Mon, 13 Mar 2023 23:20:59 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 13 Mar 2023 23:20:59 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 13 Mar 2023 23:20:59 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 13 Mar 2023 23:20:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Mar 2023 23:20:59 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd826afb15e0fb2da9a39fa76ad385840640783fb85064837ac42d7088a83f5b`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 2.7 MB (2671874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aed4622fbf41920437cd64eb0afd2873f6c133cb8a773811e7f8d02b012f0f7`  
		Last Modified: Mon, 13 Mar 2023 23:22:14 GMT  
		Size: 47.7 MB (47736083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b84895113ef8a2a181e964127bb2536c434bba757b29ffb9f2a9783f7176271`  
		Last Modified: Mon, 13 Mar 2023 23:22:07 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:a445f8de9859f39dd4c5ef2e7e8f9dffb4df793498ac89d211c7653495427364
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49350163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e092e2f9fcfc255cc6b771f7906cc910d7b643b6e8a2cbd4b0b440f533f215d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:47:18 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 13 Mar 2023 23:47:19 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 13 Mar 2023 23:47:20 GMT
ENV TELEGRAF_VERSION=1.26.0
# Mon, 13 Mar 2023 23:47:25 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 13 Mar 2023 23:47:26 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 13 Mar 2023 23:47:26 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 13 Mar 2023 23:47:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Mar 2023 23:47:27 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dab1c38052d53938443512e37031810a03849aec98af5976a010b92ee4c13c1`  
		Last Modified: Mon, 13 Mar 2023 23:48:01 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00718f537fddf7f8c80358a9bbeaac19aa91f321730dbcf5d2b3e40151cddfa`  
		Last Modified: Mon, 13 Mar 2023 23:48:01 GMT  
		Size: 2.7 MB (2704006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66bd7d8495149b7238f7f79948e7d157620679e5d2eac231656950d4c676d8f`  
		Last Modified: Mon, 13 Mar 2023 23:48:06 GMT  
		Size: 43.4 MB (43383590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1475ea4c9067111563a41ffb1c6cec63ffe29d5ca42e96c3f47efa36350869e8`  
		Last Modified: Mon, 13 Mar 2023 23:48:01 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26.0`

```console
$ docker pull telegraf@sha256:9f2974a238166819844013871b97ee75f7faabc802fef526fb2eec10916a7d76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.26.0` - linux; amd64

```console
$ docker pull telegraf@sha256:b22a40470d623b5acde30b3a4a718023dfe4fb7a4a3b0c467f4c81c4705b4d92
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137754851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2019f20bfaeecc55ae49be297185887713beca56522838df0997cfbdac6bf47f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 22:44:56 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 22:44:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 13 Mar 2023 23:20:46 GMT
ENV TELEGRAF_VERSION=1.26.0
# Mon, 13 Mar 2023 23:20:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Mon, 13 Mar 2023 23:20:50 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 13 Mar 2023 23:20:50 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Mon, 13 Mar 2023 23:20:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Mar 2023 23:20:50 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf193c1022e32f7a3ffb7be36f631ad081fb01f134f9b6b7b2affb285555deaf`  
		Last Modified: Wed, 01 Mar 2023 22:45:46 GMT  
		Size: 18.8 MB (18760000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c9df80cc94227316d89c5f6e893978f283e80e43d1e9ef432d0f63e9d55fbd`  
		Last Modified: Wed, 01 Mar 2023 22:45:42 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673fc4c4ba02a37619a21438cdcdca908b172fc42147868639db45ec3fb6c868`  
		Last Modified: Mon, 13 Mar 2023 23:21:56 GMT  
		Size: 47.9 MB (47903475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9510743483be48ca555a663080f43443280238d2e4f581a05e920f21ba0f6e55`  
		Last Modified: Mon, 13 Mar 2023 23:21:49 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26.0` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:02d25e290efa3488cb127f5b6f5f91587dbce246da83c7159256388e80d4f25e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127484742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82c0ed710458710f5cc47eb3161f37c690684de0455361eefdfb335c16559dcb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:45 GMT
ADD file:95a5e178e353a9a46c230d78b0ef83309dd487651c34e47e972ed3dae08ea00b in / 
# Wed, 01 Mar 2023 01:57:45 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:32:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:11:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:11:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 13 Mar 2023 23:32:47 GMT
ENV TELEGRAF_VERSION=1.26.0
# Mon, 13 Mar 2023 23:32:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Mon, 13 Mar 2023 23:32:54 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 13 Mar 2023 23:32:54 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Mon, 13 Mar 2023 23:32:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Mar 2023 23:32:54 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:30bee4bd8986478b5a9ecaaaba83525049f0b9b5a63ca88de878568bb6b83292`  
		Last Modified: Wed, 01 Mar 2023 02:02:32 GMT  
		Size: 50.2 MB (50212046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c2a83a9963df1d0618a3bef56d5f278e39b96940e18347e3575f30d199fb89`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 4.9 MB (4934569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6953f57698d5630bc57919975af4718f7e2eae8d6489d17ceab15dd2ab6e6`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 10.2 MB (10217796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11573ebb43311f57cffeeec94ddd828520b1890e520cdf00a9f48ba4e26fc3e6`  
		Last Modified: Thu, 02 Mar 2023 02:12:47 GMT  
		Size: 17.5 MB (17462043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ccafa66610ea2f48523ec2e133f7674459cc603987fa085111e952ed756e36`  
		Last Modified: Thu, 02 Mar 2023 02:12:44 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1446a202e285ef1da1532997410dab2bdd154bb0d0c2eaa1b1e463beaf115f`  
		Last Modified: Mon, 13 Mar 2023 23:33:28 GMT  
		Size: 44.7 MB (44656137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e54a59597676f8d916a5c25c0194baaa1a93172ecc350b71358bf929ed6eef`  
		Last Modified: Mon, 13 Mar 2023 23:33:20 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26.0` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:3dd788ec2fce2306c7ad33da4bd46d921897e0a038c031e710d70649faaf7e10
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131875171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48735df5b1fe414f8b8133972005360e4e6a9f42c5fb8a514789535110b71a2d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:49:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 17:23:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:23:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 13 Mar 2023 23:47:10 GMT
ENV TELEGRAF_VERSION=1.26.0
# Mon, 13 Mar 2023 23:47:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Mon, 13 Mar 2023 23:47:15 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 13 Mar 2023 23:47:15 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Mon, 13 Mar 2023 23:47:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Mar 2023 23:47:15 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8a090f23f28b92f40160bc1a686e3bd5cd4bbd00713a7133631cb2189575f2`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 5.2 MB (5152682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec29ff8525a3f037f4cc74d2925846a9a8c985469b4ae98fa34099110288987c`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 10.9 MB (10873588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22eb8d3d8ab6628e804f35dc6d9ebb9f557fe977afd366b59909f5114fd4c6ff`  
		Last Modified: Wed, 01 Mar 2023 17:23:38 GMT  
		Size: 18.6 MB (18598416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d38dd1a04d89bbeb2779d4abf2e671d1f39492b3df3b607f0115d47e7944b8f`  
		Last Modified: Wed, 01 Mar 2023 17:23:35 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfffa8c42f969c4305e41af97e9ffc752f1d05e717c90c69e88740f8f0107b24`  
		Last Modified: Mon, 13 Mar 2023 23:47:49 GMT  
		Size: 43.5 MB (43545118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60e9733dd9fb36a4aecc845a26c726b03079e633d5fe0869544476020c4e1fe`  
		Last Modified: Mon, 13 Mar 2023 23:47:44 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26.0-alpine`

```console
$ docker pull telegraf@sha256:07cde4c35d7b0a68485daae6f2749b7743a26d0ff01128869b9c525cd7026a53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.26.0-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:f2b25cdbc5059c3dd9c98300621363e5a4baa5c48abdff5efd18446621589ff0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53783007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b56be065cfc49ed415b7ef5b32f186d241c12dbc65da685975abf15445063485`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 13 Mar 2023 23:20:26 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 13 Mar 2023 23:20:53 GMT
ENV TELEGRAF_VERSION=1.26.0
# Mon, 13 Mar 2023 23:20:59 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 13 Mar 2023 23:20:59 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 13 Mar 2023 23:20:59 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 13 Mar 2023 23:20:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Mar 2023 23:20:59 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd826afb15e0fb2da9a39fa76ad385840640783fb85064837ac42d7088a83f5b`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 2.7 MB (2671874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aed4622fbf41920437cd64eb0afd2873f6c133cb8a773811e7f8d02b012f0f7`  
		Last Modified: Mon, 13 Mar 2023 23:22:14 GMT  
		Size: 47.7 MB (47736083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b84895113ef8a2a181e964127bb2536c434bba757b29ffb9f2a9783f7176271`  
		Last Modified: Mon, 13 Mar 2023 23:22:07 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26.0-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:a445f8de9859f39dd4c5ef2e7e8f9dffb4df793498ac89d211c7653495427364
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49350163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e092e2f9fcfc255cc6b771f7906cc910d7b643b6e8a2cbd4b0b440f533f215d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:47:18 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 13 Mar 2023 23:47:19 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 13 Mar 2023 23:47:20 GMT
ENV TELEGRAF_VERSION=1.26.0
# Mon, 13 Mar 2023 23:47:25 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 13 Mar 2023 23:47:26 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 13 Mar 2023 23:47:26 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 13 Mar 2023 23:47:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Mar 2023 23:47:27 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dab1c38052d53938443512e37031810a03849aec98af5976a010b92ee4c13c1`  
		Last Modified: Mon, 13 Mar 2023 23:48:01 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00718f537fddf7f8c80358a9bbeaac19aa91f321730dbcf5d2b3e40151cddfa`  
		Last Modified: Mon, 13 Mar 2023 23:48:01 GMT  
		Size: 2.7 MB (2704006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66bd7d8495149b7238f7f79948e7d157620679e5d2eac231656950d4c676d8f`  
		Last Modified: Mon, 13 Mar 2023 23:48:06 GMT  
		Size: 43.4 MB (43383590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1475ea4c9067111563a41ffb1c6cec63ffe29d5ca42e96c3f47efa36350869e8`  
		Last Modified: Mon, 13 Mar 2023 23:48:01 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:07cde4c35d7b0a68485daae6f2749b7743a26d0ff01128869b9c525cd7026a53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:f2b25cdbc5059c3dd9c98300621363e5a4baa5c48abdff5efd18446621589ff0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53783007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b56be065cfc49ed415b7ef5b32f186d241c12dbc65da685975abf15445063485`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 13 Mar 2023 23:20:26 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 13 Mar 2023 23:20:53 GMT
ENV TELEGRAF_VERSION=1.26.0
# Mon, 13 Mar 2023 23:20:59 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 13 Mar 2023 23:20:59 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 13 Mar 2023 23:20:59 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 13 Mar 2023 23:20:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Mar 2023 23:20:59 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd826afb15e0fb2da9a39fa76ad385840640783fb85064837ac42d7088a83f5b`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 2.7 MB (2671874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aed4622fbf41920437cd64eb0afd2873f6c133cb8a773811e7f8d02b012f0f7`  
		Last Modified: Mon, 13 Mar 2023 23:22:14 GMT  
		Size: 47.7 MB (47736083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b84895113ef8a2a181e964127bb2536c434bba757b29ffb9f2a9783f7176271`  
		Last Modified: Mon, 13 Mar 2023 23:22:07 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:a445f8de9859f39dd4c5ef2e7e8f9dffb4df793498ac89d211c7653495427364
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49350163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e092e2f9fcfc255cc6b771f7906cc910d7b643b6e8a2cbd4b0b440f533f215d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:47:18 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Mon, 13 Mar 2023 23:47:19 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Mon, 13 Mar 2023 23:47:20 GMT
ENV TELEGRAF_VERSION=1.26.0
# Mon, 13 Mar 2023 23:47:25 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 13 Mar 2023 23:47:26 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 13 Mar 2023 23:47:26 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 13 Mar 2023 23:47:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Mar 2023 23:47:27 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dab1c38052d53938443512e37031810a03849aec98af5976a010b92ee4c13c1`  
		Last Modified: Mon, 13 Mar 2023 23:48:01 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00718f537fddf7f8c80358a9bbeaac19aa91f321730dbcf5d2b3e40151cddfa`  
		Last Modified: Mon, 13 Mar 2023 23:48:01 GMT  
		Size: 2.7 MB (2704006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66bd7d8495149b7238f7f79948e7d157620679e5d2eac231656950d4c676d8f`  
		Last Modified: Mon, 13 Mar 2023 23:48:06 GMT  
		Size: 43.4 MB (43383590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1475ea4c9067111563a41ffb1c6cec63ffe29d5ca42e96c3f47efa36350869e8`  
		Last Modified: Mon, 13 Mar 2023 23:48:01 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:9f2974a238166819844013871b97ee75f7faabc802fef526fb2eec10916a7d76
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:b22a40470d623b5acde30b3a4a718023dfe4fb7a4a3b0c467f4c81c4705b4d92
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.8 MB (137754851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2019f20bfaeecc55ae49be297185887713beca56522838df0997cfbdac6bf47f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:45 GMT
ADD file:513c5d5e501279c21a05c1d8b66e5f0b02ee4b27f0b928706d92fd9ce11c1be6 in / 
# Wed, 01 Mar 2023 04:09:46 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 22:44:56 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 22:44:58 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 13 Mar 2023 23:20:46 GMT
ENV TELEGRAF_VERSION=1.26.0
# Mon, 13 Mar 2023 23:20:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Mon, 13 Mar 2023 23:20:50 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 13 Mar 2023 23:20:50 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Mon, 13 Mar 2023 23:20:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Mar 2023 23:20:50 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:32fb02163b6bb519a30f909008e852354dae10bdfd6b34190dbdfe8f15403ea0`  
		Last Modified: Wed, 01 Mar 2023 04:13:58 GMT  
		Size: 55.0 MB (55045922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167c7feebee855d117e192389484ea8367be1ba84e7ee35f4e5e5663195facbf`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 5.2 MB (5166586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6dfff1f6f3ddd2194ea0775f199572e8b2d75c38713eef0444d6b1fd0ac7604`  
		Last Modified: Wed, 01 Mar 2023 04:50:15 GMT  
		Size: 10.9 MB (10876729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf193c1022e32f7a3ffb7be36f631ad081fb01f134f9b6b7b2affb285555deaf`  
		Last Modified: Wed, 01 Mar 2023 22:45:46 GMT  
		Size: 18.8 MB (18760000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c9df80cc94227316d89c5f6e893978f283e80e43d1e9ef432d0f63e9d55fbd`  
		Last Modified: Wed, 01 Mar 2023 22:45:42 GMT  
		Size: 1.8 KB (1798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673fc4c4ba02a37619a21438cdcdca908b172fc42147868639db45ec3fb6c868`  
		Last Modified: Mon, 13 Mar 2023 23:21:56 GMT  
		Size: 47.9 MB (47903475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9510743483be48ca555a663080f43443280238d2e4f581a05e920f21ba0f6e55`  
		Last Modified: Mon, 13 Mar 2023 23:21:49 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:02d25e290efa3488cb127f5b6f5f91587dbce246da83c7159256388e80d4f25e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127484742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82c0ed710458710f5cc47eb3161f37c690684de0455361eefdfb335c16559dcb`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 01 Mar 2023 01:57:45 GMT
ADD file:95a5e178e353a9a46c230d78b0ef83309dd487651c34e47e972ed3dae08ea00b in / 
# Wed, 01 Mar 2023 01:57:45 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:32:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:32:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 02 Mar 2023 02:11:53 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Thu, 02 Mar 2023 02:11:54 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 13 Mar 2023 23:32:47 GMT
ENV TELEGRAF_VERSION=1.26.0
# Mon, 13 Mar 2023 23:32:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Mon, 13 Mar 2023 23:32:54 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 13 Mar 2023 23:32:54 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Mon, 13 Mar 2023 23:32:54 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Mar 2023 23:32:54 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:30bee4bd8986478b5a9ecaaaba83525049f0b9b5a63ca88de878568bb6b83292`  
		Last Modified: Wed, 01 Mar 2023 02:02:32 GMT  
		Size: 50.2 MB (50212046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c2a83a9963df1d0618a3bef56d5f278e39b96940e18347e3575f30d199fb89`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 4.9 MB (4934569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6953f57698d5630bc57919975af4718f7e2eae8d6489d17ceab15dd2ab6e6`  
		Last Modified: Wed, 01 Mar 2023 03:09:13 GMT  
		Size: 10.2 MB (10217796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11573ebb43311f57cffeeec94ddd828520b1890e520cdf00a9f48ba4e26fc3e6`  
		Last Modified: Thu, 02 Mar 2023 02:12:47 GMT  
		Size: 17.5 MB (17462043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ccafa66610ea2f48523ec2e133f7674459cc603987fa085111e952ed756e36`  
		Last Modified: Thu, 02 Mar 2023 02:12:44 GMT  
		Size: 1.8 KB (1806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1446a202e285ef1da1532997410dab2bdd154bb0d0c2eaa1b1e463beaf115f`  
		Last Modified: Mon, 13 Mar 2023 23:33:28 GMT  
		Size: 44.7 MB (44656137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e54a59597676f8d916a5c25c0194baaa1a93172ecc350b71358bf929ed6eef`  
		Last Modified: Mon, 13 Mar 2023 23:33:20 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:3dd788ec2fce2306c7ad33da4bd46d921897e0a038c031e710d70649faaf7e10
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131875171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48735df5b1fe414f8b8133972005360e4e6a9f42c5fb8a514789535110b71a2d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 01 Mar 2023 02:20:30 GMT
ADD file:a6a1df499d0d5b07fb366d776a11c42ddee6261e2425a921041b38e868192770 in / 
# Wed, 01 Mar 2023 02:20:30 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 02:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 02:49:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 01 Mar 2023 17:23:04 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 17:23:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Mon, 13 Mar 2023 23:47:10 GMT
ENV TELEGRAF_VERSION=1.26.0
# Mon, 13 Mar 2023 23:47:14 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Mon, 13 Mar 2023 23:47:15 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 13 Mar 2023 23:47:15 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Mon, 13 Mar 2023 23:47:15 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 13 Mar 2023 23:47:15 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:0f5fe16b1836feccd4765ac5685fc7a7b9c73445cac94fc595d2ffbc3cb59a7a`  
		Last Modified: Wed, 01 Mar 2023 02:23:53 GMT  
		Size: 53.7 MB (53703215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8a090f23f28b92f40160bc1a686e3bd5cd4bbd00713a7133631cb2189575f2`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 5.2 MB (5152682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec29ff8525a3f037f4cc74d2925846a9a8c985469b4ae98fa34099110288987c`  
		Last Modified: Wed, 01 Mar 2023 02:56:19 GMT  
		Size: 10.9 MB (10873588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22eb8d3d8ab6628e804f35dc6d9ebb9f557fe977afd366b59909f5114fd4c6ff`  
		Last Modified: Wed, 01 Mar 2023 17:23:38 GMT  
		Size: 18.6 MB (18598416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d38dd1a04d89bbeb2779d4abf2e671d1f39492b3df3b607f0115d47e7944b8f`  
		Last Modified: Wed, 01 Mar 2023 17:23:35 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfffa8c42f969c4305e41af97e9ffc752f1d05e717c90c69e88740f8f0107b24`  
		Last Modified: Mon, 13 Mar 2023 23:47:49 GMT  
		Size: 43.5 MB (43545118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60e9733dd9fb36a4aecc845a26c726b03079e633d5fe0869544476020c4e1fe`  
		Last Modified: Mon, 13 Mar 2023 23:47:44 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
