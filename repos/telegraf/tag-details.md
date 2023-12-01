<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `telegraf`

-	[`telegraf:1.26`](#telegraf126)
-	[`telegraf:1.26-alpine`](#telegraf126-alpine)
-	[`telegraf:1.26.3`](#telegraf1263)
-	[`telegraf:1.26.3-alpine`](#telegraf1263-alpine)
-	[`telegraf:1.27`](#telegraf127)
-	[`telegraf:1.27-alpine`](#telegraf127-alpine)
-	[`telegraf:1.27.4`](#telegraf1274)
-	[`telegraf:1.27.4-alpine`](#telegraf1274-alpine)
-	[`telegraf:1.28`](#telegraf128)
-	[`telegraf:1.28-alpine`](#telegraf128-alpine)
-	[`telegraf:1.28.5`](#telegraf1285)
-	[`telegraf:1.28.5-alpine`](#telegraf1285-alpine)
-	[`telegraf:alpine`](#telegrafalpine)
-	[`telegraf:latest`](#telegraflatest)

## `telegraf:1.26`

```console
$ docker pull telegraf@sha256:17b23ec44097c8703b2f80aaae2dc49ae4eb25709cda892362b4f5b03c05cef3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.26` - linux; amd64

```console
$ docker pull telegraf@sha256:c94cec5db197ca88c554703975180d5478a2555d5f145a8b4478157e7f290a61
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140137239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03411d0e0de8c0b4a0347388994e766b6609b28c1fa2786b1b99553ae294c668`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:54:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 00:55:21 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 00:55:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Nov 2023 00:55:22 GMT
ENV TELEGRAF_VERSION=1.26.3
# Wed, 22 Nov 2023 00:55:26 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Nov 2023 00:55:27 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Nov 2023 00:55:27 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 22 Nov 2023 00:55:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Nov 2023 00:55:27 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577ff23cfe55ac8872bc433ce99971a34011e7a15f7c8afa3d6492c78d6d23e5`  
		Last Modified: Tue, 21 Nov 2023 10:02:30 GMT  
		Size: 15.8 MB (15764247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383844beec9214d219a22a139caadee080d0ecd0f9a597ea3bc8082e8d029b3f`  
		Last Modified: Wed, 22 Nov 2023 00:56:18 GMT  
		Size: 18.8 MB (18760460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845ddb139da34dd72f13227e65cd6309f22b4c0eb72c78a54e662f11f6003893`  
		Last Modified: Wed, 22 Nov 2023 00:56:15 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677cfff33291336a1bc6f5df981152d7c83b66e7bc58c5a6cd66ed0c2edc2f7e`  
		Last Modified: Wed, 22 Nov 2023 00:56:23 GMT  
		Size: 50.6 MB (50552472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eba2eac29f9f17c8dbcf88964eb3a4f830342df124558a60e6590293292fe43`  
		Last Modified: Wed, 22 Nov 2023 00:56:15 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:171e96facb330f25c5bd97fed9d35e7afd299c40c78f8cf45481a4cf9e8212d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129843246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46f4211fc2d20d49d8c40fde8e6112ebe8983ff6e61163ea67ff1526eb206e22`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:54 GMT
ADD file:ed8d88d0476fad37879d872d61d05a8cffff35609566f080f78bb882d1bae26b in / 
# Tue, 21 Nov 2023 03:57:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 14:05:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 23:20:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 23:20:21 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 23:20:21 GMT
ENV TELEGRAF_VERSION=1.26.3
# Tue, 21 Nov 2023 23:20:29 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 21 Nov 2023 23:20:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 21 Nov 2023 23:20:29 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 21 Nov 2023 23:20:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 23:20:29 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:1dac19092a737e476f9b096fe28463512ae21c4f596dd2f8b84d62530416dffe`  
		Last Modified: Tue, 21 Nov 2023 04:02:11 GMT  
		Size: 50.2 MB (50215653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98461d76c0d7c5e4d320986d659d56aba23d807280d398632ef50acd8a6e028d`  
		Last Modified: Tue, 21 Nov 2023 14:15:07 GMT  
		Size: 14.9 MB (14879655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4525da0c212ff7cd23f8c7a4b0c91f33661b9d5ba480e56922393637c1b3d3`  
		Last Modified: Tue, 21 Nov 2023 23:21:20 GMT  
		Size: 17.5 MB (17463072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1294c02d3a1d783d7ee4769bb177fd8357610523a1e08b63be1cde7a65b65e6f`  
		Last Modified: Tue, 21 Nov 2023 23:21:17 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3de0157eb9518ca294285a5de508263b0a489d5776ba3a4f5523a7565ee05e`  
		Last Modified: Tue, 21 Nov 2023 23:21:25 GMT  
		Size: 47.3 MB (47282704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafc5ce30421a45cf26ea9e5822f2705e1cdb0e82bd0f362df5917014d58c532`  
		Last Modified: Tue, 21 Nov 2023 23:21:17 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:1bfe18eb4adc6f60e129d67dbc25084332bfdbca1dfe7ba00118de4d0659a27e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (134031599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b43e8aea382103f6f3b097eab0306d6cb25c6fe551accc8135bca30f1a3f9f07`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:13 GMT
ADD file:614987b9855939825ad2383e7bacbf14ea208d74906982bba3a67126702c8371 in / 
# Tue, 21 Nov 2023 06:27:13 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 01:24:17 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 01:24:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Nov 2023 01:24:19 GMT
ENV TELEGRAF_VERSION=1.26.3
# Wed, 22 Nov 2023 01:24:24 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Nov 2023 01:24:25 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Nov 2023 01:24:25 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 22 Nov 2023 01:24:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Nov 2023 01:24:25 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:bbf382c14c7b19b81c612f639e09e6a7b04eccd4481d0abac48b8ace9faae3b3`  
		Last Modified: Tue, 21 Nov 2023 06:30:47 GMT  
		Size: 53.7 MB (53707872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e860a4a6ca9e583881322c2e78baef1911e4d61bc607563e8ad9891e2d91f9`  
		Last Modified: Tue, 21 Nov 2023 08:07:01 GMT  
		Size: 15.8 MB (15750113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10006605bb4ae70273992e254de104f2d0f86488dc3181780013d8a3c68b6b82`  
		Last Modified: Wed, 22 Nov 2023 01:25:18 GMT  
		Size: 18.6 MB (18599637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1574139a6758804b66ff658a37625234608528cdac125b6da514e2d5278b0aa6`  
		Last Modified: Wed, 22 Nov 2023 01:25:16 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14187c396ed20ef566f4586a2a6e617ff7b648fd717701a1e8325aacfc3b5040`  
		Last Modified: Wed, 22 Nov 2023 01:25:21 GMT  
		Size: 46.0 MB (45971831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8fa8b6ac313053d37963ebc84b2ef9ae96ad00f8202553422b0bb9c0242166`  
		Last Modified: Wed, 22 Nov 2023 01:25:16 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26-alpine`

```console
$ docker pull telegraf@sha256:41468ab6484875506f7ddbb21522b260c5e701cacdac30bb2c58d365b8c12d0a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.26-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:44e89b6483e3ad045c83c99f1a291055367ceeffa073f50d93b159531cda8e5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.4 MB (56444230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eac521968e53994ca25a8ce57599b12d798ebf32ecc94088df341f88f5c63de5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:58 GMT
ADD file:80331a5d882ac8a70763f4b19e06f2e04ea3dca34ae6d92810815b170b3c806c in / 
# Thu, 30 Nov 2023 23:22:59 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:22:09 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 01 Dec 2023 06:00:52 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 01 Dec 2023 06:00:52 GMT
ENV TELEGRAF_VERSION=1.26.3
# Fri, 01 Dec 2023 06:01:01 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 01 Dec 2023 06:01:01 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Dec 2023 06:01:01 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Fri, 01 Dec 2023 06:01:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 06:01:01 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:1207c741d8c9b028d98c4006013f9de959da3c55f85b91ed5e4583438a0112ca`  
		Last Modified: Thu, 30 Nov 2023 23:23:40 GMT  
		Size: 3.4 MB (3379323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae43a7dfb488bfdf09941272691a16afeb9a0ec5f2aeb3afb906b9e61d0eea0`  
		Last Modified: Fri, 01 Dec 2023 05:24:18 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba8d7341b1c23b5c55532a07ae618a26f64e196b37be7f2136de99e86168abc`  
		Last Modified: Fri, 01 Dec 2023 06:01:45 GMT  
		Size: 2.7 MB (2672423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233da9243bb67caea36209a5a36b678b86583d48ee7cd7d3cfd40b009327ad05`  
		Last Modified: Fri, 01 Dec 2023 06:01:51 GMT  
		Size: 50.4 MB (50391882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415cae469aa191bf8eb2cfdf8c848ef7b90934185248c7e5a13500301ebec85a`  
		Last Modified: Fri, 01 Dec 2023 06:01:44 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:7a7da6aca0399f49b1d8d41de2c5c36fcc96c957f39ef97ec6d05b33b48d83b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51774154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e77ff943b9c16956d435bfc33d061533a36dab091f4e1faf4a4c1d6bcb4a5dd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:07 GMT
ADD file:e5c66967d6570e36da50c9d42dd8f8f55e6c6a65b92c79601ea9e750c076fa2a in / 
# Thu, 30 Nov 2023 23:11:07 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:29:18 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 01 Dec 2023 09:29:20 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 01 Dec 2023 09:29:20 GMT
ENV TELEGRAF_VERSION=1.26.3
# Fri, 01 Dec 2023 09:29:30 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 01 Dec 2023 09:29:31 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Dec 2023 09:29:31 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Fri, 01 Dec 2023 09:29:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:29:32 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b8180c93b172865af87a7c0e7e3c8bcb139e0d0c92e19c96467ff2cd4c8919ad`  
		Last Modified: Thu, 30 Nov 2023 23:11:45 GMT  
		Size: 3.3 MB (3258348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1d40317fdaf9e10db2c3b28c56f313e9d080ceaa12a39917ffdd8dffcbf3df`  
		Last Modified: Fri, 01 Dec 2023 09:30:11 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75aff9e2085fd020228bd43138ae3e332bf51dbcd4aff637cb5fba0c95df94a7`  
		Last Modified: Fri, 01 Dec 2023 09:30:12 GMT  
		Size: 2.7 MB (2702941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b8d06dc10747af3cae54030fd5d768c044d0b598cb2d694cbcac07338e8cd6`  
		Last Modified: Fri, 01 Dec 2023 09:30:17 GMT  
		Size: 45.8 MB (45812259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40e4325562197efdd7cecee9a0adc8384eb4ca03033db67c199d1c8c824aa0d`  
		Last Modified: Fri, 01 Dec 2023 09:30:11 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26.3`

```console
$ docker pull telegraf@sha256:17b23ec44097c8703b2f80aaae2dc49ae4eb25709cda892362b4f5b03c05cef3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.26.3` - linux; amd64

```console
$ docker pull telegraf@sha256:c94cec5db197ca88c554703975180d5478a2555d5f145a8b4478157e7f290a61
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140137239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03411d0e0de8c0b4a0347388994e766b6609b28c1fa2786b1b99553ae294c668`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:46 GMT
ADD file:71543995e4d314b0c86da5ddf8e0cb74649767d30b3e5b6261360de354f0567b in / 
# Tue, 21 Nov 2023 05:21:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:54:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 00:55:21 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 00:55:22 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Nov 2023 00:55:22 GMT
ENV TELEGRAF_VERSION=1.26.3
# Wed, 22 Nov 2023 00:55:26 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Nov 2023 00:55:27 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Nov 2023 00:55:27 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 22 Nov 2023 00:55:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Nov 2023 00:55:27 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:d1da99c2f14827498c4a9bb3623ae909b44564bdabad1802f064169069df81fb`  
		Last Modified: Tue, 21 Nov 2023 05:26:17 GMT  
		Size: 55.1 MB (55057903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577ff23cfe55ac8872bc433ce99971a34011e7a15f7c8afa3d6492c78d6d23e5`  
		Last Modified: Tue, 21 Nov 2023 10:02:30 GMT  
		Size: 15.8 MB (15764247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383844beec9214d219a22a139caadee080d0ecd0f9a597ea3bc8082e8d029b3f`  
		Last Modified: Wed, 22 Nov 2023 00:56:18 GMT  
		Size: 18.8 MB (18760460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845ddb139da34dd72f13227e65cd6309f22b4c0eb72c78a54e662f11f6003893`  
		Last Modified: Wed, 22 Nov 2023 00:56:15 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677cfff33291336a1bc6f5df981152d7c83b66e7bc58c5a6cd66ed0c2edc2f7e`  
		Last Modified: Wed, 22 Nov 2023 00:56:23 GMT  
		Size: 50.6 MB (50552472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eba2eac29f9f17c8dbcf88964eb3a4f830342df124558a60e6590293292fe43`  
		Last Modified: Wed, 22 Nov 2023 00:56:15 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26.3` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:171e96facb330f25c5bd97fed9d35e7afd299c40c78f8cf45481a4cf9e8212d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.8 MB (129843246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46f4211fc2d20d49d8c40fde8e6112ebe8983ff6e61163ea67ff1526eb206e22`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:54 GMT
ADD file:ed8d88d0476fad37879d872d61d05a8cffff35609566f080f78bb882d1bae26b in / 
# Tue, 21 Nov 2023 03:57:54 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 14:05:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 23:20:20 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 23:20:21 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 23:20:21 GMT
ENV TELEGRAF_VERSION=1.26.3
# Tue, 21 Nov 2023 23:20:29 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 21 Nov 2023 23:20:29 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 21 Nov 2023 23:20:29 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 21 Nov 2023 23:20:29 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 23:20:29 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:1dac19092a737e476f9b096fe28463512ae21c4f596dd2f8b84d62530416dffe`  
		Last Modified: Tue, 21 Nov 2023 04:02:11 GMT  
		Size: 50.2 MB (50215653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98461d76c0d7c5e4d320986d659d56aba23d807280d398632ef50acd8a6e028d`  
		Last Modified: Tue, 21 Nov 2023 14:15:07 GMT  
		Size: 14.9 MB (14879655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d4525da0c212ff7cd23f8c7a4b0c91f33661b9d5ba480e56922393637c1b3d3`  
		Last Modified: Tue, 21 Nov 2023 23:21:20 GMT  
		Size: 17.5 MB (17463072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1294c02d3a1d783d7ee4769bb177fd8357610523a1e08b63be1cde7a65b65e6f`  
		Last Modified: Tue, 21 Nov 2023 23:21:17 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3de0157eb9518ca294285a5de508263b0a489d5776ba3a4f5523a7565ee05e`  
		Last Modified: Tue, 21 Nov 2023 23:21:25 GMT  
		Size: 47.3 MB (47282704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafc5ce30421a45cf26ea9e5822f2705e1cdb0e82bd0f362df5917014d58c532`  
		Last Modified: Tue, 21 Nov 2023 23:21:17 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26.3` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:1bfe18eb4adc6f60e129d67dbc25084332bfdbca1dfe7ba00118de4d0659a27e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (134031599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b43e8aea382103f6f3b097eab0306d6cb25c6fe551accc8135bca30f1a3f9f07`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:13 GMT
ADD file:614987b9855939825ad2383e7bacbf14ea208d74906982bba3a67126702c8371 in / 
# Tue, 21 Nov 2023 06:27:13 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:58:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 01:24:17 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 01:24:18 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Nov 2023 01:24:19 GMT
ENV TELEGRAF_VERSION=1.26.3
# Wed, 22 Nov 2023 01:24:24 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Nov 2023 01:24:25 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Nov 2023 01:24:25 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 22 Nov 2023 01:24:25 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Nov 2023 01:24:25 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:bbf382c14c7b19b81c612f639e09e6a7b04eccd4481d0abac48b8ace9faae3b3`  
		Last Modified: Tue, 21 Nov 2023 06:30:47 GMT  
		Size: 53.7 MB (53707872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e860a4a6ca9e583881322c2e78baef1911e4d61bc607563e8ad9891e2d91f9`  
		Last Modified: Tue, 21 Nov 2023 08:07:01 GMT  
		Size: 15.8 MB (15750113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10006605bb4ae70273992e254de104f2d0f86488dc3181780013d8a3c68b6b82`  
		Last Modified: Wed, 22 Nov 2023 01:25:18 GMT  
		Size: 18.6 MB (18599637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1574139a6758804b66ff658a37625234608528cdac125b6da514e2d5278b0aa6`  
		Last Modified: Wed, 22 Nov 2023 01:25:16 GMT  
		Size: 1.8 KB (1802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14187c396ed20ef566f4586a2a6e617ff7b648fd717701a1e8325aacfc3b5040`  
		Last Modified: Wed, 22 Nov 2023 01:25:21 GMT  
		Size: 46.0 MB (45971831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8fa8b6ac313053d37963ebc84b2ef9ae96ad00f8202553422b0bb9c0242166`  
		Last Modified: Wed, 22 Nov 2023 01:25:16 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26.3-alpine`

```console
$ docker pull telegraf@sha256:41468ab6484875506f7ddbb21522b260c5e701cacdac30bb2c58d365b8c12d0a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.26.3-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:44e89b6483e3ad045c83c99f1a291055367ceeffa073f50d93b159531cda8e5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.4 MB (56444230 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eac521968e53994ca25a8ce57599b12d798ebf32ecc94088df341f88f5c63de5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:58 GMT
ADD file:80331a5d882ac8a70763f4b19e06f2e04ea3dca34ae6d92810815b170b3c806c in / 
# Thu, 30 Nov 2023 23:22:59 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:22:09 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 01 Dec 2023 06:00:52 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 01 Dec 2023 06:00:52 GMT
ENV TELEGRAF_VERSION=1.26.3
# Fri, 01 Dec 2023 06:01:01 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 01 Dec 2023 06:01:01 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Dec 2023 06:01:01 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Fri, 01 Dec 2023 06:01:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 06:01:01 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:1207c741d8c9b028d98c4006013f9de959da3c55f85b91ed5e4583438a0112ca`  
		Last Modified: Thu, 30 Nov 2023 23:23:40 GMT  
		Size: 3.4 MB (3379323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae43a7dfb488bfdf09941272691a16afeb9a0ec5f2aeb3afb906b9e61d0eea0`  
		Last Modified: Fri, 01 Dec 2023 05:24:18 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba8d7341b1c23b5c55532a07ae618a26f64e196b37be7f2136de99e86168abc`  
		Last Modified: Fri, 01 Dec 2023 06:01:45 GMT  
		Size: 2.7 MB (2672423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233da9243bb67caea36209a5a36b678b86583d48ee7cd7d3cfd40b009327ad05`  
		Last Modified: Fri, 01 Dec 2023 06:01:51 GMT  
		Size: 50.4 MB (50391882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415cae469aa191bf8eb2cfdf8c848ef7b90934185248c7e5a13500301ebec85a`  
		Last Modified: Fri, 01 Dec 2023 06:01:44 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26.3-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:7a7da6aca0399f49b1d8d41de2c5c36fcc96c957f39ef97ec6d05b33b48d83b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51774154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e77ff943b9c16956d435bfc33d061533a36dab091f4e1faf4a4c1d6bcb4a5dd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:07 GMT
ADD file:e5c66967d6570e36da50c9d42dd8f8f55e6c6a65b92c79601ea9e750c076fa2a in / 
# Thu, 30 Nov 2023 23:11:07 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 09:29:18 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 01 Dec 2023 09:29:20 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 01 Dec 2023 09:29:20 GMT
ENV TELEGRAF_VERSION=1.26.3
# Fri, 01 Dec 2023 09:29:30 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 01 Dec 2023 09:29:31 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Dec 2023 09:29:31 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Fri, 01 Dec 2023 09:29:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:29:32 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b8180c93b172865af87a7c0e7e3c8bcb139e0d0c92e19c96467ff2cd4c8919ad`  
		Last Modified: Thu, 30 Nov 2023 23:11:45 GMT  
		Size: 3.3 MB (3258348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1d40317fdaf9e10db2c3b28c56f313e9d080ceaa12a39917ffdd8dffcbf3df`  
		Last Modified: Fri, 01 Dec 2023 09:30:11 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75aff9e2085fd020228bd43138ae3e332bf51dbcd4aff637cb5fba0c95df94a7`  
		Last Modified: Fri, 01 Dec 2023 09:30:12 GMT  
		Size: 2.7 MB (2702941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60b8d06dc10747af3cae54030fd5d768c044d0b598cb2d694cbcac07338e8cd6`  
		Last Modified: Fri, 01 Dec 2023 09:30:17 GMT  
		Size: 45.8 MB (45812259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40e4325562197efdd7cecee9a0adc8384eb4ca03033db67c199d1c8c824aa0d`  
		Last Modified: Fri, 01 Dec 2023 09:30:11 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.27`

```console
$ docker pull telegraf@sha256:403ec5df85fb6a96cb6aed6c1162f34e0d46aa905fa7cda0093283125a0de586
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.27` - linux; amd64

```console
$ docker pull telegraf@sha256:3e12dc5d3ffb1611488d4613e9dbac320e90f6a1843064775f49e0d820cc70bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148105920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90c5d0e8a570fe750c23e1de7de64b69b9dc2e0bcd5f4cbea3dd8c266b13e448`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:24 GMT
ADD file:39d17d28c5de0bd629e5b7c8190228e5a445d61d668e189b7523e90e68f78244 in / 
# Tue, 21 Nov 2023 05:21:25 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:52:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 00:55:40 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 00:55:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Nov 2023 00:55:42 GMT
ENV TELEGRAF_VERSION=1.27.4
# Wed, 22 Nov 2023 00:55:46 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Nov 2023 00:55:46 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Nov 2023 00:55:47 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 22 Nov 2023 00:55:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Nov 2023 00:55:47 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:90e5e7d8b87a34877f61c2b86d053db1c4f440b9054cf49573e3be5d6a674a47`  
		Last Modified: Tue, 21 Nov 2023 05:25:34 GMT  
		Size: 49.6 MB (49582225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e1a8ca91d35598fbae8dee7f1c211f0f93cec529f6804a60e9301c53a604d0`  
		Last Modified: Tue, 21 Nov 2023 10:01:22 GMT  
		Size: 24.0 MB (24049172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7379725b6546dea0f1ba56bae82f8c5228c0e69333bc2970bd88ea89a3a8fd53`  
		Last Modified: Wed, 22 Nov 2023 00:56:35 GMT  
		Size: 19.1 MB (19145626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be681b3fe70bc00a1c9885286b51fe22faa95b1a80eb1c0a6294280523b6f08`  
		Last Modified: Wed, 22 Nov 2023 00:56:32 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd01e96edcd3f3f2bf7305a94429fd8cdc829b5be6af17ada6a4ea6c3b6e674`  
		Last Modified: Wed, 22 Nov 2023 00:56:40 GMT  
		Size: 55.3 MB (55326737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797116c75b1deaf107e348504c8b2ec8ea693e44991ff3b0036cdb0e3c1b3eee`  
		Last Modified: Wed, 22 Nov 2023 00:56:32 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:899fcbefd37a85eabc779342fa89704f2ea9ba3b22c7f1d3f8d0e8543e51837a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136631669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61a75d3e9fa662786279031d4d36bf803be6d9df7f864590d32403c0a1c3e09f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:33 GMT
ADD file:e90da0ca6ed29299007a9b8fd99fb4134cb37f22a833a55752add2b86657f694 in / 
# Tue, 21 Nov 2023 03:57:33 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 14:03:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 23:20:45 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 23:20:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 23:20:47 GMT
ENV TELEGRAF_VERSION=1.27.4
# Tue, 21 Nov 2023 23:20:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 21 Nov 2023 23:20:55 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 21 Nov 2023 23:20:55 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 21 Nov 2023 23:20:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 23:20:55 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:52c01871afffc7432976815bfd8aab1abb41e8df039231492714566f852db38a`  
		Last Modified: Tue, 21 Nov 2023 04:01:24 GMT  
		Size: 45.2 MB (45180046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cb054df5eff93daa6563e5c3e43d6288fda872fd7bdcb684c5bd0a39f4f501`  
		Last Modified: Tue, 21 Nov 2023 14:13:54 GMT  
		Size: 22.0 MB (21951942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff3d29c48da3d3c5f8514351234af2dfff8c1b36aa0f6d6914503574b0208d7`  
		Last Modified: Tue, 21 Nov 2023 23:21:38 GMT  
		Size: 18.0 MB (17991731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e82ddeb1477addeff8bbd35a93e859f9b052694676e82f072fb51df3ec9cbc3`  
		Last Modified: Tue, 21 Nov 2023 23:21:34 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f91e66476fc45ed55f69d24f9c7f37871add51201e736588c95d674bda64be6`  
		Last Modified: Tue, 21 Nov 2023 23:21:43 GMT  
		Size: 51.5 MB (51505792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f93e0e08f134aa486460e52cb94280b42ebfbbe45d48588c3bc7a6b1da91b61`  
		Last Modified: Tue, 21 Nov 2023 23:21:34 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:b0c168c7f1f4c84f6681ca01335e94dd6f5f24deb6e58e3f1b260c9c394362c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.2 MB (142238190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:537fd185a90e9ae48b968c443d776693acf144ccb3b356f2625afee3dd808495`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Nov 2023 06:26:54 GMT
ADD file:6550a7c17e64067114283d098e85f9a74d4707f2879b53c2e4cae99f329c9025 in / 
# Tue, 21 Nov 2023 06:26:55 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:57:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 01:24:38 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 01:24:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Nov 2023 01:24:39 GMT
ENV TELEGRAF_VERSION=1.27.4
# Wed, 22 Nov 2023 01:24:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Nov 2023 01:24:46 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Nov 2023 01:24:46 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 22 Nov 2023 01:24:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Nov 2023 01:24:47 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:df2021ddb7d686bdbb125598b2a6163d63035f080356b3014595f354ea0b40d6`  
		Last Modified: Tue, 21 Nov 2023 06:30:07 GMT  
		Size: 49.6 MB (49612650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d647f1dd7e741209a8a75083ccc889e39cb3e94c17f45441eae96e1a679d971`  
		Last Modified: Tue, 21 Nov 2023 08:06:01 GMT  
		Size: 23.6 MB (23584876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1d6e8fe6fcae874f25a2b1ec8d85739dcb507f15b7c7795f92b1263a3a9228`  
		Last Modified: Wed, 22 Nov 2023 01:25:33 GMT  
		Size: 19.1 MB (19079870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6061458affd69842d82b9015660b8f6e4650ce25b34b4ebbbbde61b95d8a3b13`  
		Last Modified: Wed, 22 Nov 2023 01:25:31 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdee0b2a823035808d6edac92e911520abc02003ba957b3b1fbaebd5578fef7b`  
		Last Modified: Wed, 22 Nov 2023 01:25:36 GMT  
		Size: 50.0 MB (49958636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fca8dad91bcb273eda45a21bcc806352e6b4c24477de2a203d6f5aa4f07489b`  
		Last Modified: Wed, 22 Nov 2023 01:25:31 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.27-alpine`

```console
$ docker pull telegraf@sha256:55d0f6f14d78534b95584d2f2917010d9f6f6724d160a74df316e402b1578714
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.27-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:752220ca6064313160238402e2bbf287afdf0c468fe86342cf240e5f52143458
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61200208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0798a614fd0a47663b86a66606e2493fc13a0c2550473a87f4de2386f4312596`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:23:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 01 Dec 2023 06:01:08 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 01 Dec 2023 06:01:09 GMT
ENV TELEGRAF_VERSION=1.27.4
# Fri, 01 Dec 2023 06:01:15 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 01 Dec 2023 06:01:16 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Dec 2023 06:01:16 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Fri, 01 Dec 2023 06:01:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 06:01:16 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703e958f39c4082f015dd7de32b1c116ef56e1e54010a31e991ec0c10e7feecc`  
		Last Modified: Fri, 01 Dec 2023 05:25:29 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f9134978c64af53ac70d7b738a210c1328d24dc1a25eb4d44d7173087a7a2f`  
		Last Modified: Fri, 01 Dec 2023 06:02:01 GMT  
		Size: 2.6 MB (2644946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41948024150383d83c338e84d1ffc079c6535fddc587c2f43bd78ca95cd2ae5`  
		Last Modified: Fri, 01 Dec 2023 06:02:09 GMT  
		Size: 55.2 MB (55152234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5414382c8caba775deea16a41f3091aaa31de3dafc9ff1d4567cfaf971b582`  
		Last Modified: Fri, 01 Dec 2023 06:02:01 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:81a22be451ad61262e2e845b0e952b5ecab90dcda33d0132270c8d0ebad0948e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.8 MB (55802254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9748d607314d681a98f3b3bb2ce197b6590612c303c216d466e900d82b8ff2be`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:38:30 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 01 Dec 2023 09:29:37 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 01 Dec 2023 09:29:37 GMT
ENV TELEGRAF_VERSION=1.27.4
# Fri, 01 Dec 2023 09:29:45 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 01 Dec 2023 09:29:46 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Dec 2023 09:29:46 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Fri, 01 Dec 2023 09:29:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:29:46 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f6ef2d119bdc2b844474b1941025c80c2a28072d415011a971ae3decceb4b8`  
		Last Modified: Fri, 01 Dec 2023 02:38:57 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca0a892394cd6b625d7d9cdb3d4bc69df64526779bd31ca9403a55bbbcca5c0`  
		Last Modified: Fri, 01 Dec 2023 09:30:27 GMT  
		Size: 2.7 MB (2673204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f41763daa90737683bffe594355f6ebc25c058ad7ca145f984dc1d8c142a6d`  
		Last Modified: Fri, 01 Dec 2023 09:30:32 GMT  
		Size: 49.8 MB (49795411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cea42bfc317e0b40fc34a99d9e45748b94b370205d160463aba9fbda67c27c7`  
		Last Modified: Fri, 01 Dec 2023 09:30:26 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.27.4`

```console
$ docker pull telegraf@sha256:403ec5df85fb6a96cb6aed6c1162f34e0d46aa905fa7cda0093283125a0de586
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.27.4` - linux; amd64

```console
$ docker pull telegraf@sha256:3e12dc5d3ffb1611488d4613e9dbac320e90f6a1843064775f49e0d820cc70bf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.1 MB (148105920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90c5d0e8a570fe750c23e1de7de64b69b9dc2e0bcd5f4cbea3dd8c266b13e448`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:24 GMT
ADD file:39d17d28c5de0bd629e5b7c8190228e5a445d61d668e189b7523e90e68f78244 in / 
# Tue, 21 Nov 2023 05:21:25 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:52:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 00:55:40 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 00:55:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Nov 2023 00:55:42 GMT
ENV TELEGRAF_VERSION=1.27.4
# Wed, 22 Nov 2023 00:55:46 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Nov 2023 00:55:46 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Nov 2023 00:55:47 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 22 Nov 2023 00:55:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Nov 2023 00:55:47 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:90e5e7d8b87a34877f61c2b86d053db1c4f440b9054cf49573e3be5d6a674a47`  
		Last Modified: Tue, 21 Nov 2023 05:25:34 GMT  
		Size: 49.6 MB (49582225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e1a8ca91d35598fbae8dee7f1c211f0f93cec529f6804a60e9301c53a604d0`  
		Last Modified: Tue, 21 Nov 2023 10:01:22 GMT  
		Size: 24.0 MB (24049172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7379725b6546dea0f1ba56bae82f8c5228c0e69333bc2970bd88ea89a3a8fd53`  
		Last Modified: Wed, 22 Nov 2023 00:56:35 GMT  
		Size: 19.1 MB (19145626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be681b3fe70bc00a1c9885286b51fe22faa95b1a80eb1c0a6294280523b6f08`  
		Last Modified: Wed, 22 Nov 2023 00:56:32 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbd01e96edcd3f3f2bf7305a94429fd8cdc829b5be6af17ada6a4ea6c3b6e674`  
		Last Modified: Wed, 22 Nov 2023 00:56:40 GMT  
		Size: 55.3 MB (55326737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797116c75b1deaf107e348504c8b2ec8ea693e44991ff3b0036cdb0e3c1b3eee`  
		Last Modified: Wed, 22 Nov 2023 00:56:32 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27.4` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:899fcbefd37a85eabc779342fa89704f2ea9ba3b22c7f1d3f8d0e8543e51837a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.6 MB (136631669 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61a75d3e9fa662786279031d4d36bf803be6d9df7f864590d32403c0a1c3e09f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:33 GMT
ADD file:e90da0ca6ed29299007a9b8fd99fb4134cb37f22a833a55752add2b86657f694 in / 
# Tue, 21 Nov 2023 03:57:33 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 14:03:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 23:20:45 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 23:20:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 23:20:47 GMT
ENV TELEGRAF_VERSION=1.27.4
# Tue, 21 Nov 2023 23:20:54 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 21 Nov 2023 23:20:55 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 21 Nov 2023 23:20:55 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 21 Nov 2023 23:20:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 23:20:55 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:52c01871afffc7432976815bfd8aab1abb41e8df039231492714566f852db38a`  
		Last Modified: Tue, 21 Nov 2023 04:01:24 GMT  
		Size: 45.2 MB (45180046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cb054df5eff93daa6563e5c3e43d6288fda872fd7bdcb684c5bd0a39f4f501`  
		Last Modified: Tue, 21 Nov 2023 14:13:54 GMT  
		Size: 22.0 MB (21951942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff3d29c48da3d3c5f8514351234af2dfff8c1b36aa0f6d6914503574b0208d7`  
		Last Modified: Tue, 21 Nov 2023 23:21:38 GMT  
		Size: 18.0 MB (17991731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e82ddeb1477addeff8bbd35a93e859f9b052694676e82f072fb51df3ec9cbc3`  
		Last Modified: Tue, 21 Nov 2023 23:21:34 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f91e66476fc45ed55f69d24f9c7f37871add51201e736588c95d674bda64be6`  
		Last Modified: Tue, 21 Nov 2023 23:21:43 GMT  
		Size: 51.5 MB (51505792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f93e0e08f134aa486460e52cb94280b42ebfbbe45d48588c3bc7a6b1da91b61`  
		Last Modified: Tue, 21 Nov 2023 23:21:34 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27.4` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:b0c168c7f1f4c84f6681ca01335e94dd6f5f24deb6e58e3f1b260c9c394362c7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.2 MB (142238190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:537fd185a90e9ae48b968c443d776693acf144ccb3b356f2625afee3dd808495`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Nov 2023 06:26:54 GMT
ADD file:6550a7c17e64067114283d098e85f9a74d4707f2879b53c2e4cae99f329c9025 in / 
# Tue, 21 Nov 2023 06:26:55 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:57:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 01:24:38 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 01:24:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Nov 2023 01:24:39 GMT
ENV TELEGRAF_VERSION=1.27.4
# Wed, 22 Nov 2023 01:24:45 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Nov 2023 01:24:46 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Nov 2023 01:24:46 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 22 Nov 2023 01:24:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Nov 2023 01:24:47 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:df2021ddb7d686bdbb125598b2a6163d63035f080356b3014595f354ea0b40d6`  
		Last Modified: Tue, 21 Nov 2023 06:30:07 GMT  
		Size: 49.6 MB (49612650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d647f1dd7e741209a8a75083ccc889e39cb3e94c17f45441eae96e1a679d971`  
		Last Modified: Tue, 21 Nov 2023 08:06:01 GMT  
		Size: 23.6 MB (23584876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1d6e8fe6fcae874f25a2b1ec8d85739dcb507f15b7c7795f92b1263a3a9228`  
		Last Modified: Wed, 22 Nov 2023 01:25:33 GMT  
		Size: 19.1 MB (19079870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6061458affd69842d82b9015660b8f6e4650ce25b34b4ebbbbde61b95d8a3b13`  
		Last Modified: Wed, 22 Nov 2023 01:25:31 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdee0b2a823035808d6edac92e911520abc02003ba957b3b1fbaebd5578fef7b`  
		Last Modified: Wed, 22 Nov 2023 01:25:36 GMT  
		Size: 50.0 MB (49958636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fca8dad91bcb273eda45a21bcc806352e6b4c24477de2a203d6f5aa4f07489b`  
		Last Modified: Wed, 22 Nov 2023 01:25:31 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.27.4-alpine`

```console
$ docker pull telegraf@sha256:55d0f6f14d78534b95584d2f2917010d9f6f6724d160a74df316e402b1578714
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.27.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:752220ca6064313160238402e2bbf287afdf0c468fe86342cf240e5f52143458
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61200208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0798a614fd0a47663b86a66606e2493fc13a0c2550473a87f4de2386f4312596`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:23:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 01 Dec 2023 06:01:08 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 01 Dec 2023 06:01:09 GMT
ENV TELEGRAF_VERSION=1.27.4
# Fri, 01 Dec 2023 06:01:15 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 01 Dec 2023 06:01:16 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Dec 2023 06:01:16 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Fri, 01 Dec 2023 06:01:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 06:01:16 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703e958f39c4082f015dd7de32b1c116ef56e1e54010a31e991ec0c10e7feecc`  
		Last Modified: Fri, 01 Dec 2023 05:25:29 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f9134978c64af53ac70d7b738a210c1328d24dc1a25eb4d44d7173087a7a2f`  
		Last Modified: Fri, 01 Dec 2023 06:02:01 GMT  
		Size: 2.6 MB (2644946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e41948024150383d83c338e84d1ffc079c6535fddc587c2f43bd78ca95cd2ae5`  
		Last Modified: Fri, 01 Dec 2023 06:02:09 GMT  
		Size: 55.2 MB (55152234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5414382c8caba775deea16a41f3091aaa31de3dafc9ff1d4567cfaf971b582`  
		Last Modified: Fri, 01 Dec 2023 06:02:01 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27.4-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:81a22be451ad61262e2e845b0e952b5ecab90dcda33d0132270c8d0ebad0948e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.8 MB (55802254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9748d607314d681a98f3b3bb2ce197b6590612c303c216d466e900d82b8ff2be`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:38:30 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 01 Dec 2023 09:29:37 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 01 Dec 2023 09:29:37 GMT
ENV TELEGRAF_VERSION=1.27.4
# Fri, 01 Dec 2023 09:29:45 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 01 Dec 2023 09:29:46 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Dec 2023 09:29:46 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Fri, 01 Dec 2023 09:29:46 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:29:46 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f6ef2d119bdc2b844474b1941025c80c2a28072d415011a971ae3decceb4b8`  
		Last Modified: Fri, 01 Dec 2023 02:38:57 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca0a892394cd6b625d7d9cdb3d4bc69df64526779bd31ca9403a55bbbcca5c0`  
		Last Modified: Fri, 01 Dec 2023 09:30:27 GMT  
		Size: 2.7 MB (2673204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f41763daa90737683bffe594355f6ebc25c058ad7ca145f984dc1d8c142a6d`  
		Last Modified: Fri, 01 Dec 2023 09:30:32 GMT  
		Size: 49.8 MB (49795411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cea42bfc317e0b40fc34a99d9e45748b94b370205d160463aba9fbda67c27c7`  
		Last Modified: Fri, 01 Dec 2023 09:30:26 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.28`

```console
$ docker pull telegraf@sha256:166adf9cdb9484f92fb2b83a858a069f4dfe01ffd748a1855fff259333d2f33f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.28` - linux; amd64

```console
$ docker pull telegraf@sha256:fa0fbc910ea95f36530c9feb6cc7bd46c48560a46854c1ce13ca233ea77b4ecf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.9 MB (149868209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:161be23be4a02ae5ff5db82b14e09bf372731c675b0bb8e0f176093bfbfe89dc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:24 GMT
ADD file:39d17d28c5de0bd629e5b7c8190228e5a445d61d668e189b7523e90e68f78244 in / 
# Tue, 21 Nov 2023 05:21:25 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:52:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 00:55:40 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 00:55:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Nov 2023 00:55:52 GMT
ENV TELEGRAF_VERSION=1.28.5
# Wed, 22 Nov 2023 00:55:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Nov 2023 00:55:59 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Nov 2023 00:55:59 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 22 Nov 2023 00:55:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Nov 2023 00:56:00 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:90e5e7d8b87a34877f61c2b86d053db1c4f440b9054cf49573e3be5d6a674a47`  
		Last Modified: Tue, 21 Nov 2023 05:25:34 GMT  
		Size: 49.6 MB (49582225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e1a8ca91d35598fbae8dee7f1c211f0f93cec529f6804a60e9301c53a604d0`  
		Last Modified: Tue, 21 Nov 2023 10:01:22 GMT  
		Size: 24.0 MB (24049172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7379725b6546dea0f1ba56bae82f8c5228c0e69333bc2970bd88ea89a3a8fd53`  
		Last Modified: Wed, 22 Nov 2023 00:56:35 GMT  
		Size: 19.1 MB (19145626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be681b3fe70bc00a1c9885286b51fe22faa95b1a80eb1c0a6294280523b6f08`  
		Last Modified: Wed, 22 Nov 2023 00:56:32 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55f5b8df13fa23c7d382e66f4d336730ba6f78bb1f4ced697c9601487708479`  
		Last Modified: Wed, 22 Nov 2023 00:56:57 GMT  
		Size: 57.1 MB (57089026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f328e17317df745f03d48cabb6b937264860cd55bbe71eaad7b3598cce1e9717`  
		Last Modified: Wed, 22 Nov 2023 00:56:48 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.28` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:b22442c160304fd11ee94fd355f6a226c2eef3871ad9555028a049296313e896
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137680470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f37874f14b5100b62712fdb1a68d55000ab3c0ba06969ff0b049c11a19ecd30`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:33 GMT
ADD file:e90da0ca6ed29299007a9b8fd99fb4134cb37f22a833a55752add2b86657f694 in / 
# Tue, 21 Nov 2023 03:57:33 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 14:03:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 23:20:45 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 23:20:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 23:20:58 GMT
ENV TELEGRAF_VERSION=1.28.5
# Tue, 21 Nov 2023 23:21:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 21 Nov 2023 23:21:07 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 21 Nov 2023 23:21:07 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 21 Nov 2023 23:21:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 23:21:07 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:52c01871afffc7432976815bfd8aab1abb41e8df039231492714566f852db38a`  
		Last Modified: Tue, 21 Nov 2023 04:01:24 GMT  
		Size: 45.2 MB (45180046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cb054df5eff93daa6563e5c3e43d6288fda872fd7bdcb684c5bd0a39f4f501`  
		Last Modified: Tue, 21 Nov 2023 14:13:54 GMT  
		Size: 22.0 MB (21951942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff3d29c48da3d3c5f8514351234af2dfff8c1b36aa0f6d6914503574b0208d7`  
		Last Modified: Tue, 21 Nov 2023 23:21:38 GMT  
		Size: 18.0 MB (17991731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e82ddeb1477addeff8bbd35a93e859f9b052694676e82f072fb51df3ec9cbc3`  
		Last Modified: Tue, 21 Nov 2023 23:21:34 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed7590069b1a30a172a958fcc59b4b9c1a0d7982dec6e7bbf068c35eeba027e`  
		Last Modified: Tue, 21 Nov 2023 23:22:01 GMT  
		Size: 52.6 MB (52554593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f136c69f234ebc9720d19502b2f798758f6ac2806b1448ae87eb32e577358e`  
		Last Modified: Tue, 21 Nov 2023 23:21:51 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.28` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:67bd3e3321207e3603d515c1ee779aaab29512f9ba536975d21115015ec67915
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.0 MB (144030162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cb44f54f8cc0bfe485567448df516835fa40da91cf939c9aed166b9e02fbeac`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Nov 2023 06:26:54 GMT
ADD file:6550a7c17e64067114283d098e85f9a74d4707f2879b53c2e4cae99f329c9025 in / 
# Tue, 21 Nov 2023 06:26:55 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:57:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 01:24:38 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 01:24:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Nov 2023 01:24:52 GMT
ENV TELEGRAF_VERSION=1.28.5
# Wed, 22 Nov 2023 01:24:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Nov 2023 01:24:59 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Nov 2023 01:24:59 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 22 Nov 2023 01:25:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Nov 2023 01:25:00 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:df2021ddb7d686bdbb125598b2a6163d63035f080356b3014595f354ea0b40d6`  
		Last Modified: Tue, 21 Nov 2023 06:30:07 GMT  
		Size: 49.6 MB (49612650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d647f1dd7e741209a8a75083ccc889e39cb3e94c17f45441eae96e1a679d971`  
		Last Modified: Tue, 21 Nov 2023 08:06:01 GMT  
		Size: 23.6 MB (23584876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1d6e8fe6fcae874f25a2b1ec8d85739dcb507f15b7c7795f92b1263a3a9228`  
		Last Modified: Wed, 22 Nov 2023 01:25:33 GMT  
		Size: 19.1 MB (19079870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6061458affd69842d82b9015660b8f6e4650ce25b34b4ebbbbde61b95d8a3b13`  
		Last Modified: Wed, 22 Nov 2023 01:25:31 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0d6eb6a831d90a5c2a3d778230c61d594a71333f10e605b400071fde1a1ff`  
		Last Modified: Wed, 22 Nov 2023 01:25:52 GMT  
		Size: 51.8 MB (51750608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab7e74285ef29dda0d460e79e00cdd65fe203f60ecb23b4472a2689f116717e`  
		Last Modified: Wed, 22 Nov 2023 01:25:45 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.28-alpine`

```console
$ docker pull telegraf@sha256:112eaad8a7431b370c20d3adabe4b7ac4b0b9b2f83cabcf27ae54a104bf17d59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.28-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:1193eee9874b2bce9065541569f5373d79243995f6ea9bce34056ce0425a6f6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.0 MB (62960873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bc4c6719bb3da7a75962469d87f12e5baf9f2ef5fda48fc2b05fd1d34ed878f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:23:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 01 Dec 2023 06:01:08 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 01 Dec 2023 06:01:21 GMT
ENV TELEGRAF_VERSION=1.28.5
# Fri, 01 Dec 2023 06:01:28 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 01 Dec 2023 06:01:28 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Dec 2023 06:01:28 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Fri, 01 Dec 2023 06:01:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 06:01:28 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703e958f39c4082f015dd7de32b1c116ef56e1e54010a31e991ec0c10e7feecc`  
		Last Modified: Fri, 01 Dec 2023 05:25:29 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f9134978c64af53ac70d7b738a210c1328d24dc1a25eb4d44d7173087a7a2f`  
		Last Modified: Fri, 01 Dec 2023 06:02:01 GMT  
		Size: 2.6 MB (2644946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd66689949bc0bfbc2d37396f13a4ca79202368d001d9d9919c1a2e5cb214ec`  
		Last Modified: Fri, 01 Dec 2023 06:02:30 GMT  
		Size: 56.9 MB (56912898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76b249b718bd8c689938b30cb54a35bd16c1559b0ec953bfbae3418c42dfcc1`  
		Last Modified: Fri, 01 Dec 2023 06:02:19 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.28-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:9abd92c798e7a04f30103b1c909296a6f752b93258711d6736f41565a14e77f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.6 MB (57594128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7c1be5420f2256037606879501b68b596b7270f939e5b0742cc880ce4da97cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:38:30 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 01 Dec 2023 09:29:37 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 01 Dec 2023 09:29:51 GMT
ENV TELEGRAF_VERSION=1.28.5
# Fri, 01 Dec 2023 09:29:56 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 01 Dec 2023 09:29:57 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Dec 2023 09:29:58 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Fri, 01 Dec 2023 09:29:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:29:58 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f6ef2d119bdc2b844474b1941025c80c2a28072d415011a971ae3decceb4b8`  
		Last Modified: Fri, 01 Dec 2023 02:38:57 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca0a892394cd6b625d7d9cdb3d4bc69df64526779bd31ca9403a55bbbcca5c0`  
		Last Modified: Fri, 01 Dec 2023 09:30:27 GMT  
		Size: 2.7 MB (2673204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0966c76ccd38be27a8bf79cd4f6906012dfd128984fa170f86fea2cd6155461`  
		Last Modified: Fri, 01 Dec 2023 09:30:47 GMT  
		Size: 51.6 MB (51587284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d86eebfd2c91e08ee20d44fef32c1ac56d89958f0c0ec81ddd495f2c2011698`  
		Last Modified: Fri, 01 Dec 2023 09:30:41 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.28.5`

```console
$ docker pull telegraf@sha256:166adf9cdb9484f92fb2b83a858a069f4dfe01ffd748a1855fff259333d2f33f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.28.5` - linux; amd64

```console
$ docker pull telegraf@sha256:fa0fbc910ea95f36530c9feb6cc7bd46c48560a46854c1ce13ca233ea77b4ecf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.9 MB (149868209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:161be23be4a02ae5ff5db82b14e09bf372731c675b0bb8e0f176093bfbfe89dc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:24 GMT
ADD file:39d17d28c5de0bd629e5b7c8190228e5a445d61d668e189b7523e90e68f78244 in / 
# Tue, 21 Nov 2023 05:21:25 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:52:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 00:55:40 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 00:55:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Nov 2023 00:55:52 GMT
ENV TELEGRAF_VERSION=1.28.5
# Wed, 22 Nov 2023 00:55:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Nov 2023 00:55:59 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Nov 2023 00:55:59 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 22 Nov 2023 00:55:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Nov 2023 00:56:00 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:90e5e7d8b87a34877f61c2b86d053db1c4f440b9054cf49573e3be5d6a674a47`  
		Last Modified: Tue, 21 Nov 2023 05:25:34 GMT  
		Size: 49.6 MB (49582225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e1a8ca91d35598fbae8dee7f1c211f0f93cec529f6804a60e9301c53a604d0`  
		Last Modified: Tue, 21 Nov 2023 10:01:22 GMT  
		Size: 24.0 MB (24049172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7379725b6546dea0f1ba56bae82f8c5228c0e69333bc2970bd88ea89a3a8fd53`  
		Last Modified: Wed, 22 Nov 2023 00:56:35 GMT  
		Size: 19.1 MB (19145626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be681b3fe70bc00a1c9885286b51fe22faa95b1a80eb1c0a6294280523b6f08`  
		Last Modified: Wed, 22 Nov 2023 00:56:32 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55f5b8df13fa23c7d382e66f4d336730ba6f78bb1f4ced697c9601487708479`  
		Last Modified: Wed, 22 Nov 2023 00:56:57 GMT  
		Size: 57.1 MB (57089026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f328e17317df745f03d48cabb6b937264860cd55bbe71eaad7b3598cce1e9717`  
		Last Modified: Wed, 22 Nov 2023 00:56:48 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.28.5` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:b22442c160304fd11ee94fd355f6a226c2eef3871ad9555028a049296313e896
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137680470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f37874f14b5100b62712fdb1a68d55000ab3c0ba06969ff0b049c11a19ecd30`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:33 GMT
ADD file:e90da0ca6ed29299007a9b8fd99fb4134cb37f22a833a55752add2b86657f694 in / 
# Tue, 21 Nov 2023 03:57:33 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 14:03:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 23:20:45 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 23:20:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 23:20:58 GMT
ENV TELEGRAF_VERSION=1.28.5
# Tue, 21 Nov 2023 23:21:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 21 Nov 2023 23:21:07 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 21 Nov 2023 23:21:07 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 21 Nov 2023 23:21:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 23:21:07 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:52c01871afffc7432976815bfd8aab1abb41e8df039231492714566f852db38a`  
		Last Modified: Tue, 21 Nov 2023 04:01:24 GMT  
		Size: 45.2 MB (45180046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cb054df5eff93daa6563e5c3e43d6288fda872fd7bdcb684c5bd0a39f4f501`  
		Last Modified: Tue, 21 Nov 2023 14:13:54 GMT  
		Size: 22.0 MB (21951942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff3d29c48da3d3c5f8514351234af2dfff8c1b36aa0f6d6914503574b0208d7`  
		Last Modified: Tue, 21 Nov 2023 23:21:38 GMT  
		Size: 18.0 MB (17991731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e82ddeb1477addeff8bbd35a93e859f9b052694676e82f072fb51df3ec9cbc3`  
		Last Modified: Tue, 21 Nov 2023 23:21:34 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed7590069b1a30a172a958fcc59b4b9c1a0d7982dec6e7bbf068c35eeba027e`  
		Last Modified: Tue, 21 Nov 2023 23:22:01 GMT  
		Size: 52.6 MB (52554593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f136c69f234ebc9720d19502b2f798758f6ac2806b1448ae87eb32e577358e`  
		Last Modified: Tue, 21 Nov 2023 23:21:51 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.28.5` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:67bd3e3321207e3603d515c1ee779aaab29512f9ba536975d21115015ec67915
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.0 MB (144030162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cb44f54f8cc0bfe485567448df516835fa40da91cf939c9aed166b9e02fbeac`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Nov 2023 06:26:54 GMT
ADD file:6550a7c17e64067114283d098e85f9a74d4707f2879b53c2e4cae99f329c9025 in / 
# Tue, 21 Nov 2023 06:26:55 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:57:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 01:24:38 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 01:24:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Nov 2023 01:24:52 GMT
ENV TELEGRAF_VERSION=1.28.5
# Wed, 22 Nov 2023 01:24:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Nov 2023 01:24:59 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Nov 2023 01:24:59 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 22 Nov 2023 01:25:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Nov 2023 01:25:00 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:df2021ddb7d686bdbb125598b2a6163d63035f080356b3014595f354ea0b40d6`  
		Last Modified: Tue, 21 Nov 2023 06:30:07 GMT  
		Size: 49.6 MB (49612650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d647f1dd7e741209a8a75083ccc889e39cb3e94c17f45441eae96e1a679d971`  
		Last Modified: Tue, 21 Nov 2023 08:06:01 GMT  
		Size: 23.6 MB (23584876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1d6e8fe6fcae874f25a2b1ec8d85739dcb507f15b7c7795f92b1263a3a9228`  
		Last Modified: Wed, 22 Nov 2023 01:25:33 GMT  
		Size: 19.1 MB (19079870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6061458affd69842d82b9015660b8f6e4650ce25b34b4ebbbbde61b95d8a3b13`  
		Last Modified: Wed, 22 Nov 2023 01:25:31 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0d6eb6a831d90a5c2a3d778230c61d594a71333f10e605b400071fde1a1ff`  
		Last Modified: Wed, 22 Nov 2023 01:25:52 GMT  
		Size: 51.8 MB (51750608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab7e74285ef29dda0d460e79e00cdd65fe203f60ecb23b4472a2689f116717e`  
		Last Modified: Wed, 22 Nov 2023 01:25:45 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.28.5-alpine`

```console
$ docker pull telegraf@sha256:112eaad8a7431b370c20d3adabe4b7ac4b0b9b2f83cabcf27ae54a104bf17d59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.28.5-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:1193eee9874b2bce9065541569f5373d79243995f6ea9bce34056ce0425a6f6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.0 MB (62960873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bc4c6719bb3da7a75962469d87f12e5baf9f2ef5fda48fc2b05fd1d34ed878f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:23:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 01 Dec 2023 06:01:08 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 01 Dec 2023 06:01:21 GMT
ENV TELEGRAF_VERSION=1.28.5
# Fri, 01 Dec 2023 06:01:28 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 01 Dec 2023 06:01:28 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Dec 2023 06:01:28 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Fri, 01 Dec 2023 06:01:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 06:01:28 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703e958f39c4082f015dd7de32b1c116ef56e1e54010a31e991ec0c10e7feecc`  
		Last Modified: Fri, 01 Dec 2023 05:25:29 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f9134978c64af53ac70d7b738a210c1328d24dc1a25eb4d44d7173087a7a2f`  
		Last Modified: Fri, 01 Dec 2023 06:02:01 GMT  
		Size: 2.6 MB (2644946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd66689949bc0bfbc2d37396f13a4ca79202368d001d9d9919c1a2e5cb214ec`  
		Last Modified: Fri, 01 Dec 2023 06:02:30 GMT  
		Size: 56.9 MB (56912898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76b249b718bd8c689938b30cb54a35bd16c1559b0ec953bfbae3418c42dfcc1`  
		Last Modified: Fri, 01 Dec 2023 06:02:19 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.28.5-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:9abd92c798e7a04f30103b1c909296a6f752b93258711d6736f41565a14e77f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.6 MB (57594128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7c1be5420f2256037606879501b68b596b7270f939e5b0742cc880ce4da97cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:38:30 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 01 Dec 2023 09:29:37 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 01 Dec 2023 09:29:51 GMT
ENV TELEGRAF_VERSION=1.28.5
# Fri, 01 Dec 2023 09:29:56 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 01 Dec 2023 09:29:57 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Dec 2023 09:29:58 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Fri, 01 Dec 2023 09:29:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:29:58 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f6ef2d119bdc2b844474b1941025c80c2a28072d415011a971ae3decceb4b8`  
		Last Modified: Fri, 01 Dec 2023 02:38:57 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca0a892394cd6b625d7d9cdb3d4bc69df64526779bd31ca9403a55bbbcca5c0`  
		Last Modified: Fri, 01 Dec 2023 09:30:27 GMT  
		Size: 2.7 MB (2673204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0966c76ccd38be27a8bf79cd4f6906012dfd128984fa170f86fea2cd6155461`  
		Last Modified: Fri, 01 Dec 2023 09:30:47 GMT  
		Size: 51.6 MB (51587284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d86eebfd2c91e08ee20d44fef32c1ac56d89958f0c0ec81ddd495f2c2011698`  
		Last Modified: Fri, 01 Dec 2023 09:30:41 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:112eaad8a7431b370c20d3adabe4b7ac4b0b9b2f83cabcf27ae54a104bf17d59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:1193eee9874b2bce9065541569f5373d79243995f6ea9bce34056ce0425a6f6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.0 MB (62960873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bc4c6719bb3da7a75962469d87f12e5baf9f2ef5fda48fc2b05fd1d34ed878f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:23:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 01 Dec 2023 06:01:08 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 01 Dec 2023 06:01:21 GMT
ENV TELEGRAF_VERSION=1.28.5
# Fri, 01 Dec 2023 06:01:28 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 01 Dec 2023 06:01:28 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Dec 2023 06:01:28 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Fri, 01 Dec 2023 06:01:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 06:01:28 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703e958f39c4082f015dd7de32b1c116ef56e1e54010a31e991ec0c10e7feecc`  
		Last Modified: Fri, 01 Dec 2023 05:25:29 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f9134978c64af53ac70d7b738a210c1328d24dc1a25eb4d44d7173087a7a2f`  
		Last Modified: Fri, 01 Dec 2023 06:02:01 GMT  
		Size: 2.6 MB (2644946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd66689949bc0bfbc2d37396f13a4ca79202368d001d9d9919c1a2e5cb214ec`  
		Last Modified: Fri, 01 Dec 2023 06:02:30 GMT  
		Size: 56.9 MB (56912898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76b249b718bd8c689938b30cb54a35bd16c1559b0ec953bfbae3418c42dfcc1`  
		Last Modified: Fri, 01 Dec 2023 06:02:19 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:9abd92c798e7a04f30103b1c909296a6f752b93258711d6736f41565a14e77f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.6 MB (57594128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7c1be5420f2256037606879501b68b596b7270f939e5b0742cc880ce4da97cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:38:30 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 01 Dec 2023 09:29:37 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 01 Dec 2023 09:29:51 GMT
ENV TELEGRAF_VERSION=1.28.5
# Fri, 01 Dec 2023 09:29:56 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 01 Dec 2023 09:29:57 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Dec 2023 09:29:58 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Fri, 01 Dec 2023 09:29:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:29:58 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f6ef2d119bdc2b844474b1941025c80c2a28072d415011a971ae3decceb4b8`  
		Last Modified: Fri, 01 Dec 2023 02:38:57 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca0a892394cd6b625d7d9cdb3d4bc69df64526779bd31ca9403a55bbbcca5c0`  
		Last Modified: Fri, 01 Dec 2023 09:30:27 GMT  
		Size: 2.7 MB (2673204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0966c76ccd38be27a8bf79cd4f6906012dfd128984fa170f86fea2cd6155461`  
		Last Modified: Fri, 01 Dec 2023 09:30:47 GMT  
		Size: 51.6 MB (51587284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d86eebfd2c91e08ee20d44fef32c1ac56d89958f0c0ec81ddd495f2c2011698`  
		Last Modified: Fri, 01 Dec 2023 09:30:41 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:166adf9cdb9484f92fb2b83a858a069f4dfe01ffd748a1855fff259333d2f33f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:fa0fbc910ea95f36530c9feb6cc7bd46c48560a46854c1ce13ca233ea77b4ecf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.9 MB (149868209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:161be23be4a02ae5ff5db82b14e09bf372731c675b0bb8e0f176093bfbfe89dc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:24 GMT
ADD file:39d17d28c5de0bd629e5b7c8190228e5a445d61d668e189b7523e90e68f78244 in / 
# Tue, 21 Nov 2023 05:21:25 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 09:52:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 00:55:40 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 00:55:42 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Nov 2023 00:55:52 GMT
ENV TELEGRAF_VERSION=1.28.5
# Wed, 22 Nov 2023 00:55:59 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Nov 2023 00:55:59 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Nov 2023 00:55:59 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 22 Nov 2023 00:55:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Nov 2023 00:56:00 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:90e5e7d8b87a34877f61c2b86d053db1c4f440b9054cf49573e3be5d6a674a47`  
		Last Modified: Tue, 21 Nov 2023 05:25:34 GMT  
		Size: 49.6 MB (49582225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e1a8ca91d35598fbae8dee7f1c211f0f93cec529f6804a60e9301c53a604d0`  
		Last Modified: Tue, 21 Nov 2023 10:01:22 GMT  
		Size: 24.0 MB (24049172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7379725b6546dea0f1ba56bae82f8c5228c0e69333bc2970bd88ea89a3a8fd53`  
		Last Modified: Wed, 22 Nov 2023 00:56:35 GMT  
		Size: 19.1 MB (19145626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be681b3fe70bc00a1c9885286b51fe22faa95b1a80eb1c0a6294280523b6f08`  
		Last Modified: Wed, 22 Nov 2023 00:56:32 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e55f5b8df13fa23c7d382e66f4d336730ba6f78bb1f4ced697c9601487708479`  
		Last Modified: Wed, 22 Nov 2023 00:56:57 GMT  
		Size: 57.1 MB (57089026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f328e17317df745f03d48cabb6b937264860cd55bbe71eaad7b3598cce1e9717`  
		Last Modified: Wed, 22 Nov 2023 00:56:48 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:b22442c160304fd11ee94fd355f6a226c2eef3871ad9555028a049296313e896
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137680470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f37874f14b5100b62712fdb1a68d55000ab3c0ba06969ff0b049c11a19ecd30`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Nov 2023 03:57:33 GMT
ADD file:e90da0ca6ed29299007a9b8fd99fb4134cb37f22a833a55752add2b86657f694 in / 
# Tue, 21 Nov 2023 03:57:33 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 14:03:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 23:20:45 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 23:20:46 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 21 Nov 2023 23:20:58 GMT
ENV TELEGRAF_VERSION=1.28.5
# Tue, 21 Nov 2023 23:21:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 21 Nov 2023 23:21:07 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 21 Nov 2023 23:21:07 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 21 Nov 2023 23:21:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 21 Nov 2023 23:21:07 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:52c01871afffc7432976815bfd8aab1abb41e8df039231492714566f852db38a`  
		Last Modified: Tue, 21 Nov 2023 04:01:24 GMT  
		Size: 45.2 MB (45180046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6cb054df5eff93daa6563e5c3e43d6288fda872fd7bdcb684c5bd0a39f4f501`  
		Last Modified: Tue, 21 Nov 2023 14:13:54 GMT  
		Size: 22.0 MB (21951942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ff3d29c48da3d3c5f8514351234af2dfff8c1b36aa0f6d6914503574b0208d7`  
		Last Modified: Tue, 21 Nov 2023 23:21:38 GMT  
		Size: 18.0 MB (17991731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e82ddeb1477addeff8bbd35a93e859f9b052694676e82f072fb51df3ec9cbc3`  
		Last Modified: Tue, 21 Nov 2023 23:21:34 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed7590069b1a30a172a958fcc59b4b9c1a0d7982dec6e7bbf068c35eeba027e`  
		Last Modified: Tue, 21 Nov 2023 23:22:01 GMT  
		Size: 52.6 MB (52554593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f136c69f234ebc9720d19502b2f798758f6ac2806b1448ae87eb32e577358e`  
		Last Modified: Tue, 21 Nov 2023 23:21:51 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:67bd3e3321207e3603d515c1ee779aaab29512f9ba536975d21115015ec67915
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.0 MB (144030162 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cb44f54f8cc0bfe485567448df516835fa40da91cf939c9aed166b9e02fbeac`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 21 Nov 2023 06:26:54 GMT
ADD file:6550a7c17e64067114283d098e85f9a74d4707f2879b53c2e4cae99f329c9025 in / 
# Tue, 21 Nov 2023 06:26:55 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:57:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 01:24:38 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 22 Nov 2023 01:24:39 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 22 Nov 2023 01:24:52 GMT
ENV TELEGRAF_VERSION=1.28.5
# Wed, 22 Nov 2023 01:24:58 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 22 Nov 2023 01:24:59 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 22 Nov 2023 01:24:59 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 22 Nov 2023 01:25:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 22 Nov 2023 01:25:00 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:df2021ddb7d686bdbb125598b2a6163d63035f080356b3014595f354ea0b40d6`  
		Last Modified: Tue, 21 Nov 2023 06:30:07 GMT  
		Size: 49.6 MB (49612650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d647f1dd7e741209a8a75083ccc889e39cb3e94c17f45441eae96e1a679d971`  
		Last Modified: Tue, 21 Nov 2023 08:06:01 GMT  
		Size: 23.6 MB (23584876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1d6e8fe6fcae874f25a2b1ec8d85739dcb507f15b7c7795f92b1263a3a9228`  
		Last Modified: Wed, 22 Nov 2023 01:25:33 GMT  
		Size: 19.1 MB (19079870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6061458affd69842d82b9015660b8f6e4650ce25b34b4ebbbbde61b95d8a3b13`  
		Last Modified: Wed, 22 Nov 2023 01:25:31 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f0d6eb6a831d90a5c2a3d778230c61d594a71333f10e605b400071fde1a1ff`  
		Last Modified: Wed, 22 Nov 2023 01:25:52 GMT  
		Size: 51.8 MB (51750608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab7e74285ef29dda0d460e79e00cdd65fe203f60ecb23b4472a2689f116717e`  
		Last Modified: Wed, 22 Nov 2023 01:25:45 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
