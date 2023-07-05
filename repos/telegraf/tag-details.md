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
-	[`telegraf:1.27.1`](#telegraf1271)
-	[`telegraf:1.27.1-alpine`](#telegraf1271-alpine)
-	[`telegraf:alpine`](#telegrafalpine)
-	[`telegraf:latest`](#telegraflatest)

## `telegraf:1.25`

```console
$ docker pull telegraf@sha256:657a164708f19f93718276016e40b3501562119efcdcb7bfdd8427a0dc0612d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.25` - linux; amd64

```console
$ docker pull telegraf@sha256:062b01d233ebfa566f3238d859d02b3ad7317ea1b74838aba1d953cab0b787ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.2 MB (136154360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22f736ab17d3c2e2cf7d8c676022a9746b755c0303b667ef14da46168a34d016`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:09 GMT
ADD file:b7c0be2bb90e88689b1c16da78dea0b85760b55b90ef2e5bc4a529c89e4fa25b in / 
# Tue, 04 Jul 2023 01:20:10 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:30:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:16:11 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:16:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 04 Jul 2023 23:16:12 GMT
ENV TELEGRAF_VERSION=1.25.3
# Tue, 04 Jul 2023 23:16:17 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 04 Jul 2023 23:16:17 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 04 Jul 2023 23:16:17 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 04 Jul 2023 23:16:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 23:16:17 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:34df401c391c7595044379e04e8ad4856a5a3974cdbf5a160f0a204d761e88aa`  
		Last Modified: Tue, 04 Jul 2023 01:25:21 GMT  
		Size: 55.1 MB (55055300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdd0e5b72ccae203ec30d533c0bcd34200af90265e0531c66356812e529af32`  
		Last Modified: Tue, 04 Jul 2023 03:52:30 GMT  
		Size: 15.8 MB (15760327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdd6a8cbbe7f0c0ce19dfd327a6ea351abb20d37232ff4f8b52034911c5160`  
		Last Modified: Tue, 04 Jul 2023 23:17:03 GMT  
		Size: 18.8 MB (18759976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e9a2cf04848eecc0f6636054dba0ffc8dd35224a847057a12e01ead6c233d2`  
		Last Modified: Tue, 04 Jul 2023 23:17:01 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5efe9779331511ea6d1eb6c10cd67b29e7f235e4a3b5cbc7b94acb5524bf7920`  
		Last Modified: Tue, 04 Jul 2023 23:17:08 GMT  
		Size: 46.6 MB (46576607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5cc9e87ad0ec6184d209e932018abe416c8f83e219743ec7e4f06c7974698c`  
		Last Modified: Tue, 04 Jul 2023 23:17:00 GMT  
		Size: 342.0 B  
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
$ docker pull telegraf@sha256:0cddea82f609d86121b031dd75b919d33816af53c8cb214f7afd8537d92f2dee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130366592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8c3abafa9ffb7eea67608e89591db0ac6995e043560363d747b3658470fbd04`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:43 GMT
ADD file:e626446584d8094b7b58d72a717380ca64d3e9ab924fc625406fe26a83fe1d8b in / 
# Tue, 04 Jul 2023 01:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:56:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:50:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:50:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 04 Jul 2023 23:50:01 GMT
ENV TELEGRAF_VERSION=1.25.3
# Tue, 04 Jul 2023 23:50:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 04 Jul 2023 23:50:07 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 04 Jul 2023 23:50:07 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 04 Jul 2023 23:50:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 23:50:07 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:29279ac7c19f9c667f1c6b07bfba6fba20ca0d945b9fbc6edad6f75d13361fae`  
		Last Modified: Tue, 04 Jul 2023 02:01:38 GMT  
		Size: 53.7 MB (53703979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0c3fcc5367be60f92df0774820f317a179565cd3ee9c222f5500a7be32151e`  
		Last Modified: Tue, 04 Jul 2023 06:22:01 GMT  
		Size: 15.7 MB (15746747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83d195ed9213dade8d68e377e1e3f201dcc9db5e4db236b185c97f593d9685e`  
		Last Modified: Tue, 04 Jul 2023 23:50:46 GMT  
		Size: 18.6 MB (18598537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71eecde55db05e6ff5b4e60e55dbd1384f71e3c2d4256a02804eaf7348f1c6f6`  
		Last Modified: Tue, 04 Jul 2023 23:50:44 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9703e0001931ed7b0cac85c30d4773d9b77bf62333c1d02f4a4ab9ea5d56ca37`  
		Last Modified: Tue, 04 Jul 2023 23:50:49 GMT  
		Size: 42.3 MB (42315178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd42925e3fc803c7fef27ebffdc55173c9aa42505b5af529fd774e81697d3f0`  
		Last Modified: Tue, 04 Jul 2023 23:50:44 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25-alpine`

```console
$ docker pull telegraf@sha256:0ab1ee27391df8eca074482b539b9aee5d6b2e6d2986e4040675ea1771c24827
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.25-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:4af6029141ed5e65ebb3f5854545be8804f378158d3ea8ca86cc164cd250f7e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52439734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d95ea10154c5b631dc30528e8022d2b8505ffbabc247b69d8a8c68ea22bf16e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 04:23:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Thu, 15 Jun 2023 04:23:01 GMT
ENV TELEGRAF_VERSION=1.25.3
# Thu, 15 Jun 2023 04:23:07 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Thu, 15 Jun 2023 04:23:07 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 15 Jun 2023 04:23:07 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Thu, 15 Jun 2023 04:23:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 04:23:08 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5e43bc5fa99e35cf47b43ea5bc4251b51bb08c70ce9c0b15270878ef2a0963`  
		Last Modified: Thu, 15 Jun 2023 04:23:52 GMT  
		Size: 2.7 MB (2671752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb243cfb4afaf2eb52159e92f52f16a523278ba3191a2821105f9bc5ab551e1`  
		Last Modified: Thu, 15 Jun 2023 04:23:59 GMT  
		Size: 46.4 MB (46392665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e2908126481e9bcbc296e89036faf1af309d7d7d17c50ccf9d5eab2145d52a5`  
		Last Modified: Thu, 15 Jun 2023 04:23:52 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25.3`

```console
$ docker pull telegraf@sha256:657a164708f19f93718276016e40b3501562119efcdcb7bfdd8427a0dc0612d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.25.3` - linux; amd64

```console
$ docker pull telegraf@sha256:062b01d233ebfa566f3238d859d02b3ad7317ea1b74838aba1d953cab0b787ad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.2 MB (136154360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22f736ab17d3c2e2cf7d8c676022a9746b755c0303b667ef14da46168a34d016`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:09 GMT
ADD file:b7c0be2bb90e88689b1c16da78dea0b85760b55b90ef2e5bc4a529c89e4fa25b in / 
# Tue, 04 Jul 2023 01:20:10 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:30:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:16:11 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:16:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 04 Jul 2023 23:16:12 GMT
ENV TELEGRAF_VERSION=1.25.3
# Tue, 04 Jul 2023 23:16:17 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 04 Jul 2023 23:16:17 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 04 Jul 2023 23:16:17 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 04 Jul 2023 23:16:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 23:16:17 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:34df401c391c7595044379e04e8ad4856a5a3974cdbf5a160f0a204d761e88aa`  
		Last Modified: Tue, 04 Jul 2023 01:25:21 GMT  
		Size: 55.1 MB (55055300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdd0e5b72ccae203ec30d533c0bcd34200af90265e0531c66356812e529af32`  
		Last Modified: Tue, 04 Jul 2023 03:52:30 GMT  
		Size: 15.8 MB (15760327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdd6a8cbbe7f0c0ce19dfd327a6ea351abb20d37232ff4f8b52034911c5160`  
		Last Modified: Tue, 04 Jul 2023 23:17:03 GMT  
		Size: 18.8 MB (18759976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e9a2cf04848eecc0f6636054dba0ffc8dd35224a847057a12e01ead6c233d2`  
		Last Modified: Tue, 04 Jul 2023 23:17:01 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5efe9779331511ea6d1eb6c10cd67b29e7f235e4a3b5cbc7b94acb5524bf7920`  
		Last Modified: Tue, 04 Jul 2023 23:17:08 GMT  
		Size: 46.6 MB (46576607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc5cc9e87ad0ec6184d209e932018abe416c8f83e219743ec7e4f06c7974698c`  
		Last Modified: Tue, 04 Jul 2023 23:17:00 GMT  
		Size: 342.0 B  
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
$ docker pull telegraf@sha256:0cddea82f609d86121b031dd75b919d33816af53c8cb214f7afd8537d92f2dee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.4 MB (130366592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8c3abafa9ffb7eea67608e89591db0ac6995e043560363d747b3658470fbd04`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:43 GMT
ADD file:e626446584d8094b7b58d72a717380ca64d3e9ab924fc625406fe26a83fe1d8b in / 
# Tue, 04 Jul 2023 01:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:56:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:50:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:50:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 04 Jul 2023 23:50:01 GMT
ENV TELEGRAF_VERSION=1.25.3
# Tue, 04 Jul 2023 23:50:06 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 04 Jul 2023 23:50:07 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 04 Jul 2023 23:50:07 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 04 Jul 2023 23:50:07 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 23:50:07 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:29279ac7c19f9c667f1c6b07bfba6fba20ca0d945b9fbc6edad6f75d13361fae`  
		Last Modified: Tue, 04 Jul 2023 02:01:38 GMT  
		Size: 53.7 MB (53703979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0c3fcc5367be60f92df0774820f317a179565cd3ee9c222f5500a7be32151e`  
		Last Modified: Tue, 04 Jul 2023 06:22:01 GMT  
		Size: 15.7 MB (15746747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83d195ed9213dade8d68e377e1e3f201dcc9db5e4db236b185c97f593d9685e`  
		Last Modified: Tue, 04 Jul 2023 23:50:46 GMT  
		Size: 18.6 MB (18598537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71eecde55db05e6ff5b4e60e55dbd1384f71e3c2d4256a02804eaf7348f1c6f6`  
		Last Modified: Tue, 04 Jul 2023 23:50:44 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9703e0001931ed7b0cac85c30d4773d9b77bf62333c1d02f4a4ab9ea5d56ca37`  
		Last Modified: Tue, 04 Jul 2023 23:50:49 GMT  
		Size: 42.3 MB (42315178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd42925e3fc803c7fef27ebffdc55173c9aa42505b5af529fd774e81697d3f0`  
		Last Modified: Tue, 04 Jul 2023 23:50:44 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25.3-alpine`

```console
$ docker pull telegraf@sha256:0ab1ee27391df8eca074482b539b9aee5d6b2e6d2986e4040675ea1771c24827
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.25.3-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:4af6029141ed5e65ebb3f5854545be8804f378158d3ea8ca86cc164cd250f7e0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.4 MB (52439734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d95ea10154c5b631dc30528e8022d2b8505ffbabc247b69d8a8c68ea22bf16e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 04:23:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Thu, 15 Jun 2023 04:23:01 GMT
ENV TELEGRAF_VERSION=1.25.3
# Thu, 15 Jun 2023 04:23:07 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Thu, 15 Jun 2023 04:23:07 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 15 Jun 2023 04:23:07 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Thu, 15 Jun 2023 04:23:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 04:23:08 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5e43bc5fa99e35cf47b43ea5bc4251b51bb08c70ce9c0b15270878ef2a0963`  
		Last Modified: Thu, 15 Jun 2023 04:23:52 GMT  
		Size: 2.7 MB (2671752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acb243cfb4afaf2eb52159e92f52f16a523278ba3191a2821105f9bc5ab551e1`  
		Last Modified: Thu, 15 Jun 2023 04:23:59 GMT  
		Size: 46.4 MB (46392665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e2908126481e9bcbc296e89036faf1af309d7d7d17c50ccf9d5eab2145d52a5`  
		Last Modified: Thu, 15 Jun 2023 04:23:52 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26`

```console
$ docker pull telegraf@sha256:95e14f9427ec525eb191fd46b8e55d89e3a2940327214d71b22c676042c90b7c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.26` - linux; amd64

```console
$ docker pull telegraf@sha256:f2885b63cc61014db28f8d8c9a2a27ad0e7a2773c953de973bccc59c23ccef70
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140130262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2387d21c0a6291f53a6662047b2501de2bbc1f8dfd54c20bb646cd2d46f47cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:09 GMT
ADD file:b7c0be2bb90e88689b1c16da78dea0b85760b55b90ef2e5bc4a529c89e4fa25b in / 
# Tue, 04 Jul 2023 01:20:10 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:30:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:16:11 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:16:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 04 Jul 2023 23:16:25 GMT
ENV TELEGRAF_VERSION=1.26.3
# Tue, 04 Jul 2023 23:16:31 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 04 Jul 2023 23:16:31 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 04 Jul 2023 23:16:31 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 04 Jul 2023 23:16:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 23:16:31 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:34df401c391c7595044379e04e8ad4856a5a3974cdbf5a160f0a204d761e88aa`  
		Last Modified: Tue, 04 Jul 2023 01:25:21 GMT  
		Size: 55.1 MB (55055300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdd0e5b72ccae203ec30d533c0bcd34200af90265e0531c66356812e529af32`  
		Last Modified: Tue, 04 Jul 2023 03:52:30 GMT  
		Size: 15.8 MB (15760327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdd6a8cbbe7f0c0ce19dfd327a6ea351abb20d37232ff4f8b52034911c5160`  
		Last Modified: Tue, 04 Jul 2023 23:17:03 GMT  
		Size: 18.8 MB (18759976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e9a2cf04848eecc0f6636054dba0ffc8dd35224a847057a12e01ead6c233d2`  
		Last Modified: Tue, 04 Jul 2023 23:17:01 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187fd15dd610e4622b13d2ed644c8af9f422c9047dcc24fc5e37a00265ca77f2`  
		Last Modified: Tue, 04 Jul 2023 23:17:28 GMT  
		Size: 50.6 MB (50552511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b67bf983282fb2b80e8d2f8a57e3ba8e39b7471046fb37ce91321ae42730e43`  
		Last Modified: Tue, 04 Jul 2023 23:17:20 GMT  
		Size: 340.0 B  
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
$ docker pull telegraf@sha256:85c28b96f06356d5068694069fb86f0704d619176192b25a6dd46aceee16cb23
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (134023231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3540359f6562e6958b6c4b747e2ee250bed5450ffbf19968d252d57112d06cd3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:43 GMT
ADD file:e626446584d8094b7b58d72a717380ca64d3e9ab924fc625406fe26a83fe1d8b in / 
# Tue, 04 Jul 2023 01:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:56:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:50:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:50:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 04 Jul 2023 23:50:09 GMT
ENV TELEGRAF_VERSION=1.26.3
# Tue, 04 Jul 2023 23:50:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 04 Jul 2023 23:50:20 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 04 Jul 2023 23:50:20 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 04 Jul 2023 23:50:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 23:50:20 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:29279ac7c19f9c667f1c6b07bfba6fba20ca0d945b9fbc6edad6f75d13361fae`  
		Last Modified: Tue, 04 Jul 2023 02:01:38 GMT  
		Size: 53.7 MB (53703979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0c3fcc5367be60f92df0774820f317a179565cd3ee9c222f5500a7be32151e`  
		Last Modified: Tue, 04 Jul 2023 06:22:01 GMT  
		Size: 15.7 MB (15746747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83d195ed9213dade8d68e377e1e3f201dcc9db5e4db236b185c97f593d9685e`  
		Last Modified: Tue, 04 Jul 2023 23:50:46 GMT  
		Size: 18.6 MB (18598537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71eecde55db05e6ff5b4e60e55dbd1384f71e3c2d4256a02804eaf7348f1c6f6`  
		Last Modified: Tue, 04 Jul 2023 23:50:44 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c54514a46a98a3704d27332b689ad884640335654de45b9acf7fd3b9c57f41d`  
		Last Modified: Tue, 04 Jul 2023 23:51:02 GMT  
		Size: 46.0 MB (45971815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcbfcb584bf6da0a206de1e78a3c5b75608a622df9fb1a7287e51768356e987`  
		Last Modified: Tue, 04 Jul 2023 23:50:57 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26-alpine`

```console
$ docker pull telegraf@sha256:d7670fca45a2fa0c153447618c85b9648ee58b55b0e4c9803ed5ede3ae027160
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.26-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:4fe69f57d5b57f7419e6120e28b665bcaa4bd1b25e0e29c38ddd44c6219f33af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.4 MB (56439016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b17e2edadcd01dd98f9dcd6f7f9f21fc64ae2cc415a8ea360fdb844ebcd82ad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 04:23:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Thu, 15 Jun 2023 04:23:13 GMT
ENV TELEGRAF_VERSION=1.26.3
# Thu, 15 Jun 2023 04:23:21 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Thu, 15 Jun 2023 04:23:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 15 Jun 2023 04:23:22 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Thu, 15 Jun 2023 04:23:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 04:23:22 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5e43bc5fa99e35cf47b43ea5bc4251b51bb08c70ce9c0b15270878ef2a0963`  
		Last Modified: Thu, 15 Jun 2023 04:23:52 GMT  
		Size: 2.7 MB (2671752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18990458155a92d1fb3fae8eed5615af4d63beeb00fa44a5fbd158977f7ef425`  
		Last Modified: Thu, 15 Jun 2023 04:24:18 GMT  
		Size: 50.4 MB (50391945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4274a4d20dcdf6dd563418735d039dffa8131530660a69c32270923f6c62b9ea`  
		Last Modified: Thu, 15 Jun 2023 04:24:09 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:5de71a2aa2f231e2710b08014fadaece7fae2a0dec3d6deee41269608eef2c55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51777920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24d87a2fbcaeb6bd28afc599e0c730ea53207fed335061771bd62f9408750015`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:02:51 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 07:08:51 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Thu, 15 Jun 2023 07:08:51 GMT
ENV TELEGRAF_VERSION=1.26.3
# Thu, 15 Jun 2023 07:08:58 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Thu, 15 Jun 2023 07:08:59 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 15 Jun 2023 07:08:59 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Thu, 15 Jun 2023 07:08:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 07:08:59 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a2405a5350060a5def51b41b8304bf174521998b815b48c87250c4ba922453`  
		Last Modified: Thu, 15 Jun 2023 03:03:19 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533040d8d2939a14e08289606aa07e7e8b93b273b0cc9bbdc66c5e5bae7901dd`  
		Last Modified: Thu, 15 Jun 2023 07:09:27 GMT  
		Size: 2.7 MB (2703885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75ae3de250799144d4a3ad82b891ea2058ef091277e638c7c82e4609d815a8e`  
		Last Modified: Thu, 15 Jun 2023 07:09:31 GMT  
		Size: 45.8 MB (45812293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f27b13bf3f7b32f2842c148833f64deb24dead30665ae31f7224f4313ba9872`  
		Last Modified: Thu, 15 Jun 2023 07:09:26 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26.3`

```console
$ docker pull telegraf@sha256:95e14f9427ec525eb191fd46b8e55d89e3a2940327214d71b22c676042c90b7c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.26.3` - linux; amd64

```console
$ docker pull telegraf@sha256:f2885b63cc61014db28f8d8c9a2a27ad0e7a2773c953de973bccc59c23ccef70
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.1 MB (140130262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2387d21c0a6291f53a6662047b2501de2bbc1f8dfd54c20bb646cd2d46f47cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:09 GMT
ADD file:b7c0be2bb90e88689b1c16da78dea0b85760b55b90ef2e5bc4a529c89e4fa25b in / 
# Tue, 04 Jul 2023 01:20:10 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:30:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:16:11 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:16:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 04 Jul 2023 23:16:25 GMT
ENV TELEGRAF_VERSION=1.26.3
# Tue, 04 Jul 2023 23:16:31 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 04 Jul 2023 23:16:31 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 04 Jul 2023 23:16:31 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 04 Jul 2023 23:16:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 23:16:31 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:34df401c391c7595044379e04e8ad4856a5a3974cdbf5a160f0a204d761e88aa`  
		Last Modified: Tue, 04 Jul 2023 01:25:21 GMT  
		Size: 55.1 MB (55055300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdd0e5b72ccae203ec30d533c0bcd34200af90265e0531c66356812e529af32`  
		Last Modified: Tue, 04 Jul 2023 03:52:30 GMT  
		Size: 15.8 MB (15760327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdd6a8cbbe7f0c0ce19dfd327a6ea351abb20d37232ff4f8b52034911c5160`  
		Last Modified: Tue, 04 Jul 2023 23:17:03 GMT  
		Size: 18.8 MB (18759976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e9a2cf04848eecc0f6636054dba0ffc8dd35224a847057a12e01ead6c233d2`  
		Last Modified: Tue, 04 Jul 2023 23:17:01 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187fd15dd610e4622b13d2ed644c8af9f422c9047dcc24fc5e37a00265ca77f2`  
		Last Modified: Tue, 04 Jul 2023 23:17:28 GMT  
		Size: 50.6 MB (50552511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b67bf983282fb2b80e8d2f8a57e3ba8e39b7471046fb37ce91321ae42730e43`  
		Last Modified: Tue, 04 Jul 2023 23:17:20 GMT  
		Size: 340.0 B  
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
$ docker pull telegraf@sha256:85c28b96f06356d5068694069fb86f0704d619176192b25a6dd46aceee16cb23
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.0 MB (134023231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3540359f6562e6958b6c4b747e2ee250bed5450ffbf19968d252d57112d06cd3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:43 GMT
ADD file:e626446584d8094b7b58d72a717380ca64d3e9ab924fc625406fe26a83fe1d8b in / 
# Tue, 04 Jul 2023 01:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:56:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:50:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:50:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 04 Jul 2023 23:50:09 GMT
ENV TELEGRAF_VERSION=1.26.3
# Tue, 04 Jul 2023 23:50:19 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 04 Jul 2023 23:50:20 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 04 Jul 2023 23:50:20 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 04 Jul 2023 23:50:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 23:50:20 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:29279ac7c19f9c667f1c6b07bfba6fba20ca0d945b9fbc6edad6f75d13361fae`  
		Last Modified: Tue, 04 Jul 2023 02:01:38 GMT  
		Size: 53.7 MB (53703979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0c3fcc5367be60f92df0774820f317a179565cd3ee9c222f5500a7be32151e`  
		Last Modified: Tue, 04 Jul 2023 06:22:01 GMT  
		Size: 15.7 MB (15746747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83d195ed9213dade8d68e377e1e3f201dcc9db5e4db236b185c97f593d9685e`  
		Last Modified: Tue, 04 Jul 2023 23:50:46 GMT  
		Size: 18.6 MB (18598537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71eecde55db05e6ff5b4e60e55dbd1384f71e3c2d4256a02804eaf7348f1c6f6`  
		Last Modified: Tue, 04 Jul 2023 23:50:44 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c54514a46a98a3704d27332b689ad884640335654de45b9acf7fd3b9c57f41d`  
		Last Modified: Tue, 04 Jul 2023 23:51:02 GMT  
		Size: 46.0 MB (45971815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcbfcb584bf6da0a206de1e78a3c5b75608a622df9fb1a7287e51768356e987`  
		Last Modified: Tue, 04 Jul 2023 23:50:57 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26.3-alpine`

```console
$ docker pull telegraf@sha256:d7670fca45a2fa0c153447618c85b9648ee58b55b0e4c9803ed5ede3ae027160
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.26.3-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:4fe69f57d5b57f7419e6120e28b665bcaa4bd1b25e0e29c38ddd44c6219f33af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.4 MB (56439016 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b17e2edadcd01dd98f9dcd6f7f9f21fc64ae2cc415a8ea360fdb844ebcd82ad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 04:23:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Thu, 15 Jun 2023 04:23:13 GMT
ENV TELEGRAF_VERSION=1.26.3
# Thu, 15 Jun 2023 04:23:21 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Thu, 15 Jun 2023 04:23:22 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 15 Jun 2023 04:23:22 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Thu, 15 Jun 2023 04:23:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 04:23:22 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5e43bc5fa99e35cf47b43ea5bc4251b51bb08c70ce9c0b15270878ef2a0963`  
		Last Modified: Thu, 15 Jun 2023 04:23:52 GMT  
		Size: 2.7 MB (2671752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18990458155a92d1fb3fae8eed5615af4d63beeb00fa44a5fbd158977f7ef425`  
		Last Modified: Thu, 15 Jun 2023 04:24:18 GMT  
		Size: 50.4 MB (50391945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4274a4d20dcdf6dd563418735d039dffa8131530660a69c32270923f6c62b9ea`  
		Last Modified: Thu, 15 Jun 2023 04:24:09 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26.3-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:5de71a2aa2f231e2710b08014fadaece7fae2a0dec3d6deee41269608eef2c55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51777920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24d87a2fbcaeb6bd28afc599e0c730ea53207fed335061771bd62f9408750015`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:02:51 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 07:08:51 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Thu, 15 Jun 2023 07:08:51 GMT
ENV TELEGRAF_VERSION=1.26.3
# Thu, 15 Jun 2023 07:08:58 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Thu, 15 Jun 2023 07:08:59 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 15 Jun 2023 07:08:59 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Thu, 15 Jun 2023 07:08:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 15 Jun 2023 07:08:59 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a2405a5350060a5def51b41b8304bf174521998b815b48c87250c4ba922453`  
		Last Modified: Thu, 15 Jun 2023 03:03:19 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533040d8d2939a14e08289606aa07e7e8b93b273b0cc9bbdc66c5e5bae7901dd`  
		Last Modified: Thu, 15 Jun 2023 07:09:27 GMT  
		Size: 2.7 MB (2703885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75ae3de250799144d4a3ad82b891ea2058ef091277e638c7c82e4609d815a8e`  
		Last Modified: Thu, 15 Jun 2023 07:09:31 GMT  
		Size: 45.8 MB (45812293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f27b13bf3f7b32f2842c148833f64deb24dead30665ae31f7224f4313ba9872`  
		Last Modified: Thu, 15 Jun 2023 07:09:26 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.27`

```console
$ docker pull telegraf@sha256:c65c745bb6fc27494154d96a88ba35f544a41004941a05e79f76ab8814fe8db2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.27` - linux; amd64

```console
$ docker pull telegraf@sha256:1ce21e13d48bb476b09a3cad3b7b9b97b34fb1c7a0581e51b94ef05efc4c88b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.2 MB (143175627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:878f80ac97840d4e09bf96699924e28408ea2d67eb2872e14e22521a51735c13`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:09 GMT
ADD file:b7c0be2bb90e88689b1c16da78dea0b85760b55b90ef2e5bc4a529c89e4fa25b in / 
# Tue, 04 Jul 2023 01:20:10 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:30:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:16:11 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:16:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 04 Jul 2023 23:16:36 GMT
ENV TELEGRAF_VERSION=1.27.1
# Tue, 04 Jul 2023 23:16:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 04 Jul 2023 23:16:43 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 04 Jul 2023 23:16:43 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 04 Jul 2023 23:16:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 23:16:43 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:34df401c391c7595044379e04e8ad4856a5a3974cdbf5a160f0a204d761e88aa`  
		Last Modified: Tue, 04 Jul 2023 01:25:21 GMT  
		Size: 55.1 MB (55055300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdd0e5b72ccae203ec30d533c0bcd34200af90265e0531c66356812e529af32`  
		Last Modified: Tue, 04 Jul 2023 03:52:30 GMT  
		Size: 15.8 MB (15760327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdd6a8cbbe7f0c0ce19dfd327a6ea351abb20d37232ff4f8b52034911c5160`  
		Last Modified: Tue, 04 Jul 2023 23:17:03 GMT  
		Size: 18.8 MB (18759976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e9a2cf04848eecc0f6636054dba0ffc8dd35224a847057a12e01ead6c233d2`  
		Last Modified: Tue, 04 Jul 2023 23:17:01 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c238740b06acf5a94e2666bbef6e0ec0ec8d94147656b68a992c7760040d70`  
		Last Modified: Tue, 04 Jul 2023 23:17:46 GMT  
		Size: 53.6 MB (53597872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ab6f24935e35c33081717fbc5666ca6fabf4b15968b2e62f999c3272c2a2a4`  
		Last Modified: Tue, 04 Jul 2023 23:17:37 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:302c9a60e14cf51d88aef9fc16643c87c043616cf4ed8aeb3d122ae2a12b278a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.7 MB (132724303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39ad8ecfc38b2ffcffe3dc0d4428f47dac2b0a71407fe61ebea0d7dcbcece34e`
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
# Thu, 22 Jun 2023 01:07:33 GMT
ENV TELEGRAF_VERSION=1.27.1
# Thu, 22 Jun 2023 01:07:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 22 Jun 2023 01:07:41 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 22 Jun 2023 01:07:41 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 22 Jun 2023 01:07:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Jun 2023 01:07:42 GMT
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
	-	`sha256:3ee249d2105f4f54938949c9068ac69a22f46a9cacded630be2d0fcef55ae03b`  
		Last Modified: Thu, 22 Jun 2023 01:08:01 GMT  
		Size: 50.2 MB (50173147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51cbe6e4cd83e9913d7e5d38e6e0d3ae00e2ce250e7a8027eaf256e6ad6edae8`  
		Last Modified: Thu, 22 Jun 2023 01:07:53 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:06a53774993759ec7d1b8dbb3b3ebabfd6f84f7d81422324e9c59988fb349553
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.8 MB (136804102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf41418b9da855cf0aeaabbfd595ca0ebec4e8c2a5337d89316d059f599168d4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:43 GMT
ADD file:e626446584d8094b7b58d72a717380ca64d3e9ab924fc625406fe26a83fe1d8b in / 
# Tue, 04 Jul 2023 01:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:56:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:50:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:50:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 04 Jul 2023 23:50:24 GMT
ENV TELEGRAF_VERSION=1.27.1
# Tue, 04 Jul 2023 23:50:29 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 04 Jul 2023 23:50:30 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 04 Jul 2023 23:50:30 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 04 Jul 2023 23:50:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 23:50:30 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:29279ac7c19f9c667f1c6b07bfba6fba20ca0d945b9fbc6edad6f75d13361fae`  
		Last Modified: Tue, 04 Jul 2023 02:01:38 GMT  
		Size: 53.7 MB (53703979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0c3fcc5367be60f92df0774820f317a179565cd3ee9c222f5500a7be32151e`  
		Last Modified: Tue, 04 Jul 2023 06:22:01 GMT  
		Size: 15.7 MB (15746747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83d195ed9213dade8d68e377e1e3f201dcc9db5e4db236b185c97f593d9685e`  
		Last Modified: Tue, 04 Jul 2023 23:50:46 GMT  
		Size: 18.6 MB (18598537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71eecde55db05e6ff5b4e60e55dbd1384f71e3c2d4256a02804eaf7348f1c6f6`  
		Last Modified: Tue, 04 Jul 2023 23:50:44 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb05d1e3693bac15fa4b4278eca59528e675f55de77bda988bb25ceab35206dd`  
		Last Modified: Tue, 04 Jul 2023 23:51:17 GMT  
		Size: 48.8 MB (48752687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d951f91bfb3b996e0fbfd7cc299a5330ba2f9e43ae268d3d04e0c6eba7257cf`  
		Last Modified: Tue, 04 Jul 2023 23:51:11 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.27-alpine`

```console
$ docker pull telegraf@sha256:4b14e6faf48105345abf53298eba59762d947fb2488de3d1c76b9ee359ffb8f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.27-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:59cd83c07d16cbeff3af83aba30fc06d6f3a23b736c3ddec79927e7281a2f476
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59470173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ccbe7242f733e2cf4440dc20ca993e91f5d6e4ba6b930b804afc5cef9a8957`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 04:23:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 21 Jun 2023 22:20:30 GMT
ENV TELEGRAF_VERSION=1.27.1
# Wed, 21 Jun 2023 22:20:36 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 21 Jun 2023 22:20:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 21 Jun 2023 22:20:36 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 21 Jun 2023 22:20:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 21 Jun 2023 22:20:37 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5e43bc5fa99e35cf47b43ea5bc4251b51bb08c70ce9c0b15270878ef2a0963`  
		Last Modified: Thu, 15 Jun 2023 04:23:52 GMT  
		Size: 2.7 MB (2671752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb248cbd630eaeed38ce9aa0ce52fd183e239fa1f80592d27e88e3a2fc3f48f`  
		Last Modified: Wed, 21 Jun 2023 22:21:24 GMT  
		Size: 53.4 MB (53423102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cfd83eafaa01ab3bc445acd89d18a61e9f0b5bdd0ca12cb3284b92599819ad`  
		Last Modified: Wed, 21 Jun 2023 22:21:16 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:f761259202b930f609136cf2c90d6afd8e09d9e9b6977a04494cf3e637833a5c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54546606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:071a85b3224b44f06d2fe0a775feb73fc7f6c90c3d52918c5b180749d35f5664`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:02:51 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 07:08:51 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 21 Jun 2023 22:42:26 GMT
ENV TELEGRAF_VERSION=1.27.1
# Wed, 21 Jun 2023 22:42:34 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 21 Jun 2023 22:42:35 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 21 Jun 2023 22:42:35 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 21 Jun 2023 22:42:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 21 Jun 2023 22:42:35 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a2405a5350060a5def51b41b8304bf174521998b815b48c87250c4ba922453`  
		Last Modified: Thu, 15 Jun 2023 03:03:19 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533040d8d2939a14e08289606aa07e7e8b93b273b0cc9bbdc66c5e5bae7901dd`  
		Last Modified: Thu, 15 Jun 2023 07:09:27 GMT  
		Size: 2.7 MB (2703885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdaadc0d318d859694ed0718fd99239f59dd7c94685383c38a7887e7dfddcd35`  
		Last Modified: Wed, 21 Jun 2023 22:43:17 GMT  
		Size: 48.6 MB (48580976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c41b5ba8ffcf610a3f2fd335a8ced7a45cd6107b8ee5f89ff4d67532f5ce7bea`  
		Last Modified: Wed, 21 Jun 2023 22:43:12 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.27.1`

```console
$ docker pull telegraf@sha256:c65c745bb6fc27494154d96a88ba35f544a41004941a05e79f76ab8814fe8db2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.27.1` - linux; amd64

```console
$ docker pull telegraf@sha256:1ce21e13d48bb476b09a3cad3b7b9b97b34fb1c7a0581e51b94ef05efc4c88b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.2 MB (143175627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:878f80ac97840d4e09bf96699924e28408ea2d67eb2872e14e22521a51735c13`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:09 GMT
ADD file:b7c0be2bb90e88689b1c16da78dea0b85760b55b90ef2e5bc4a529c89e4fa25b in / 
# Tue, 04 Jul 2023 01:20:10 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:30:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:16:11 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:16:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 04 Jul 2023 23:16:36 GMT
ENV TELEGRAF_VERSION=1.27.1
# Tue, 04 Jul 2023 23:16:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 04 Jul 2023 23:16:43 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 04 Jul 2023 23:16:43 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 04 Jul 2023 23:16:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 23:16:43 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:34df401c391c7595044379e04e8ad4856a5a3974cdbf5a160f0a204d761e88aa`  
		Last Modified: Tue, 04 Jul 2023 01:25:21 GMT  
		Size: 55.1 MB (55055300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdd0e5b72ccae203ec30d533c0bcd34200af90265e0531c66356812e529af32`  
		Last Modified: Tue, 04 Jul 2023 03:52:30 GMT  
		Size: 15.8 MB (15760327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdd6a8cbbe7f0c0ce19dfd327a6ea351abb20d37232ff4f8b52034911c5160`  
		Last Modified: Tue, 04 Jul 2023 23:17:03 GMT  
		Size: 18.8 MB (18759976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e9a2cf04848eecc0f6636054dba0ffc8dd35224a847057a12e01ead6c233d2`  
		Last Modified: Tue, 04 Jul 2023 23:17:01 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c238740b06acf5a94e2666bbef6e0ec0ec8d94147656b68a992c7760040d70`  
		Last Modified: Tue, 04 Jul 2023 23:17:46 GMT  
		Size: 53.6 MB (53597872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ab6f24935e35c33081717fbc5666ca6fabf4b15968b2e62f999c3272c2a2a4`  
		Last Modified: Tue, 04 Jul 2023 23:17:37 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27.1` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:302c9a60e14cf51d88aef9fc16643c87c043616cf4ed8aeb3d122ae2a12b278a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.7 MB (132724303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39ad8ecfc38b2ffcffe3dc0d4428f47dac2b0a71407fe61ebea0d7dcbcece34e`
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
# Thu, 22 Jun 2023 01:07:33 GMT
ENV TELEGRAF_VERSION=1.27.1
# Thu, 22 Jun 2023 01:07:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 22 Jun 2023 01:07:41 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 22 Jun 2023 01:07:41 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 22 Jun 2023 01:07:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Jun 2023 01:07:42 GMT
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
	-	`sha256:3ee249d2105f4f54938949c9068ac69a22f46a9cacded630be2d0fcef55ae03b`  
		Last Modified: Thu, 22 Jun 2023 01:08:01 GMT  
		Size: 50.2 MB (50173147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51cbe6e4cd83e9913d7e5d38e6e0d3ae00e2ce250e7a8027eaf256e6ad6edae8`  
		Last Modified: Thu, 22 Jun 2023 01:07:53 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27.1` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:06a53774993759ec7d1b8dbb3b3ebabfd6f84f7d81422324e9c59988fb349553
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.8 MB (136804102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf41418b9da855cf0aeaabbfd595ca0ebec4e8c2a5337d89316d059f599168d4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:43 GMT
ADD file:e626446584d8094b7b58d72a717380ca64d3e9ab924fc625406fe26a83fe1d8b in / 
# Tue, 04 Jul 2023 01:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:56:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:50:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:50:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 04 Jul 2023 23:50:24 GMT
ENV TELEGRAF_VERSION=1.27.1
# Tue, 04 Jul 2023 23:50:29 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 04 Jul 2023 23:50:30 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 04 Jul 2023 23:50:30 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 04 Jul 2023 23:50:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 23:50:30 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:29279ac7c19f9c667f1c6b07bfba6fba20ca0d945b9fbc6edad6f75d13361fae`  
		Last Modified: Tue, 04 Jul 2023 02:01:38 GMT  
		Size: 53.7 MB (53703979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0c3fcc5367be60f92df0774820f317a179565cd3ee9c222f5500a7be32151e`  
		Last Modified: Tue, 04 Jul 2023 06:22:01 GMT  
		Size: 15.7 MB (15746747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83d195ed9213dade8d68e377e1e3f201dcc9db5e4db236b185c97f593d9685e`  
		Last Modified: Tue, 04 Jul 2023 23:50:46 GMT  
		Size: 18.6 MB (18598537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71eecde55db05e6ff5b4e60e55dbd1384f71e3c2d4256a02804eaf7348f1c6f6`  
		Last Modified: Tue, 04 Jul 2023 23:50:44 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb05d1e3693bac15fa4b4278eca59528e675f55de77bda988bb25ceab35206dd`  
		Last Modified: Tue, 04 Jul 2023 23:51:17 GMT  
		Size: 48.8 MB (48752687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d951f91bfb3b996e0fbfd7cc299a5330ba2f9e43ae268d3d04e0c6eba7257cf`  
		Last Modified: Tue, 04 Jul 2023 23:51:11 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.27.1-alpine`

```console
$ docker pull telegraf@sha256:4b14e6faf48105345abf53298eba59762d947fb2488de3d1c76b9ee359ffb8f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.27.1-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:59cd83c07d16cbeff3af83aba30fc06d6f3a23b736c3ddec79927e7281a2f476
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59470173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ccbe7242f733e2cf4440dc20ca993e91f5d6e4ba6b930b804afc5cef9a8957`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 04:23:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 21 Jun 2023 22:20:30 GMT
ENV TELEGRAF_VERSION=1.27.1
# Wed, 21 Jun 2023 22:20:36 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 21 Jun 2023 22:20:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 21 Jun 2023 22:20:36 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 21 Jun 2023 22:20:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 21 Jun 2023 22:20:37 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5e43bc5fa99e35cf47b43ea5bc4251b51bb08c70ce9c0b15270878ef2a0963`  
		Last Modified: Thu, 15 Jun 2023 04:23:52 GMT  
		Size: 2.7 MB (2671752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb248cbd630eaeed38ce9aa0ce52fd183e239fa1f80592d27e88e3a2fc3f48f`  
		Last Modified: Wed, 21 Jun 2023 22:21:24 GMT  
		Size: 53.4 MB (53423102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cfd83eafaa01ab3bc445acd89d18a61e9f0b5bdd0ca12cb3284b92599819ad`  
		Last Modified: Wed, 21 Jun 2023 22:21:16 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.27.1-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:f761259202b930f609136cf2c90d6afd8e09d9e9b6977a04494cf3e637833a5c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54546606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:071a85b3224b44f06d2fe0a775feb73fc7f6c90c3d52918c5b180749d35f5664`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:02:51 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 07:08:51 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 21 Jun 2023 22:42:26 GMT
ENV TELEGRAF_VERSION=1.27.1
# Wed, 21 Jun 2023 22:42:34 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 21 Jun 2023 22:42:35 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 21 Jun 2023 22:42:35 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 21 Jun 2023 22:42:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 21 Jun 2023 22:42:35 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a2405a5350060a5def51b41b8304bf174521998b815b48c87250c4ba922453`  
		Last Modified: Thu, 15 Jun 2023 03:03:19 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533040d8d2939a14e08289606aa07e7e8b93b273b0cc9bbdc66c5e5bae7901dd`  
		Last Modified: Thu, 15 Jun 2023 07:09:27 GMT  
		Size: 2.7 MB (2703885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdaadc0d318d859694ed0718fd99239f59dd7c94685383c38a7887e7dfddcd35`  
		Last Modified: Wed, 21 Jun 2023 22:43:17 GMT  
		Size: 48.6 MB (48580976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c41b5ba8ffcf610a3f2fd335a8ced7a45cd6107b8ee5f89ff4d67532f5ce7bea`  
		Last Modified: Wed, 21 Jun 2023 22:43:12 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:4b14e6faf48105345abf53298eba59762d947fb2488de3d1c76b9ee359ffb8f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:59cd83c07d16cbeff3af83aba30fc06d6f3a23b736c3ddec79927e7281a2f476
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59470173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ccbe7242f733e2cf4440dc20ca993e91f5d6e4ba6b930b804afc5cef9a8957`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:09:36 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 04:23:01 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 21 Jun 2023 22:20:30 GMT
ENV TELEGRAF_VERSION=1.27.1
# Wed, 21 Jun 2023 22:20:36 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 21 Jun 2023 22:20:36 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 21 Jun 2023 22:20:36 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 21 Jun 2023 22:20:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 21 Jun 2023 22:20:37 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2214dfdd928ecf1e62b4f8e2a9a59608a27026918bc2c56798c200b89a66607`  
		Last Modified: Thu, 15 Jun 2023 00:11:46 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d5e43bc5fa99e35cf47b43ea5bc4251b51bb08c70ce9c0b15270878ef2a0963`  
		Last Modified: Thu, 15 Jun 2023 04:23:52 GMT  
		Size: 2.7 MB (2671752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb248cbd630eaeed38ce9aa0ce52fd183e239fa1f80592d27e88e3a2fc3f48f`  
		Last Modified: Wed, 21 Jun 2023 22:21:24 GMT  
		Size: 53.4 MB (53423102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8cfd83eafaa01ab3bc445acd89d18a61e9f0b5bdd0ca12cb3284b92599819ad`  
		Last Modified: Wed, 21 Jun 2023 22:21:16 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:f761259202b930f609136cf2c90d6afd8e09d9e9b6977a04494cf3e637833a5c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.5 MB (54546606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:071a85b3224b44f06d2fe0a775feb73fc7f6c90c3d52918c5b180749d35f5664`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:02:51 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 15 Jun 2023 07:08:51 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Wed, 21 Jun 2023 22:42:26 GMT
ENV TELEGRAF_VERSION=1.27.1
# Wed, 21 Jun 2023 22:42:34 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Wed, 21 Jun 2023 22:42:35 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 21 Jun 2023 22:42:35 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Wed, 21 Jun 2023 22:42:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 21 Jun 2023 22:42:35 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66a2405a5350060a5def51b41b8304bf174521998b815b48c87250c4ba922453`  
		Last Modified: Thu, 15 Jun 2023 03:03:19 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533040d8d2939a14e08289606aa07e7e8b93b273b0cc9bbdc66c5e5bae7901dd`  
		Last Modified: Thu, 15 Jun 2023 07:09:27 GMT  
		Size: 2.7 MB (2703885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdaadc0d318d859694ed0718fd99239f59dd7c94685383c38a7887e7dfddcd35`  
		Last Modified: Wed, 21 Jun 2023 22:43:17 GMT  
		Size: 48.6 MB (48580976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c41b5ba8ffcf610a3f2fd335a8ced7a45cd6107b8ee5f89ff4d67532f5ce7bea`  
		Last Modified: Wed, 21 Jun 2023 22:43:12 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:c65c745bb6fc27494154d96a88ba35f544a41004941a05e79f76ab8814fe8db2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:1ce21e13d48bb476b09a3cad3b7b9b97b34fb1c7a0581e51b94ef05efc4c88b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.2 MB (143175627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:878f80ac97840d4e09bf96699924e28408ea2d67eb2872e14e22521a51735c13`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 04 Jul 2023 01:20:09 GMT
ADD file:b7c0be2bb90e88689b1c16da78dea0b85760b55b90ef2e5bc4a529c89e4fa25b in / 
# Tue, 04 Jul 2023 01:20:10 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 03:30:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:16:11 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:16:12 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 04 Jul 2023 23:16:36 GMT
ENV TELEGRAF_VERSION=1.27.1
# Tue, 04 Jul 2023 23:16:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 04 Jul 2023 23:16:43 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 04 Jul 2023 23:16:43 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 04 Jul 2023 23:16:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 23:16:43 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:34df401c391c7595044379e04e8ad4856a5a3974cdbf5a160f0a204d761e88aa`  
		Last Modified: Tue, 04 Jul 2023 01:25:21 GMT  
		Size: 55.1 MB (55055300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fdd0e5b72ccae203ec30d533c0bcd34200af90265e0531c66356812e529af32`  
		Last Modified: Tue, 04 Jul 2023 03:52:30 GMT  
		Size: 15.8 MB (15760327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cdd6a8cbbe7f0c0ce19dfd327a6ea351abb20d37232ff4f8b52034911c5160`  
		Last Modified: Tue, 04 Jul 2023 23:17:03 GMT  
		Size: 18.8 MB (18759976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e9a2cf04848eecc0f6636054dba0ffc8dd35224a847057a12e01ead6c233d2`  
		Last Modified: Tue, 04 Jul 2023 23:17:01 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c238740b06acf5a94e2666bbef6e0ec0ec8d94147656b68a992c7760040d70`  
		Last Modified: Tue, 04 Jul 2023 23:17:46 GMT  
		Size: 53.6 MB (53597872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3ab6f24935e35c33081717fbc5666ca6fabf4b15968b2e62f999c3272c2a2a4`  
		Last Modified: Tue, 04 Jul 2023 23:17:37 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:302c9a60e14cf51d88aef9fc16643c87c043616cf4ed8aeb3d122ae2a12b278a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.7 MB (132724303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39ad8ecfc38b2ffcffe3dc0d4428f47dac2b0a71407fe61ebea0d7dcbcece34e`
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
# Thu, 22 Jun 2023 01:07:33 GMT
ENV TELEGRAF_VERSION=1.27.1
# Thu, 22 Jun 2023 01:07:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Thu, 22 Jun 2023 01:07:41 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 22 Jun 2023 01:07:41 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Thu, 22 Jun 2023 01:07:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Jun 2023 01:07:42 GMT
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
	-	`sha256:3ee249d2105f4f54938949c9068ac69a22f46a9cacded630be2d0fcef55ae03b`  
		Last Modified: Thu, 22 Jun 2023 01:08:01 GMT  
		Size: 50.2 MB (50173147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51cbe6e4cd83e9913d7e5d38e6e0d3ae00e2ce250e7a8027eaf256e6ad6edae8`  
		Last Modified: Thu, 22 Jun 2023 01:07:53 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:06a53774993759ec7d1b8dbb3b3ebabfd6f84f7d81422324e9c59988fb349553
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.8 MB (136804102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf41418b9da855cf0aeaabbfd595ca0ebec4e8c2a5337d89316d059f599168d4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 04 Jul 2023 01:57:43 GMT
ADD file:e626446584d8094b7b58d72a717380ca64d3e9ab924fc625406fe26a83fe1d8b in / 
# Tue, 04 Jul 2023 01:57:43 GMT
CMD ["bash"]
# Tue, 04 Jul 2023 05:56:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:50:00 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 23:50:01 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Tue, 04 Jul 2023 23:50:24 GMT
ENV TELEGRAF_VERSION=1.27.1
# Tue, 04 Jul 2023 23:50:29 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Tue, 04 Jul 2023 23:50:30 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 04 Jul 2023 23:50:30 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Tue, 04 Jul 2023 23:50:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 04 Jul 2023 23:50:30 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:29279ac7c19f9c667f1c6b07bfba6fba20ca0d945b9fbc6edad6f75d13361fae`  
		Last Modified: Tue, 04 Jul 2023 02:01:38 GMT  
		Size: 53.7 MB (53703979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0c3fcc5367be60f92df0774820f317a179565cd3ee9c222f5500a7be32151e`  
		Last Modified: Tue, 04 Jul 2023 06:22:01 GMT  
		Size: 15.7 MB (15746747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83d195ed9213dade8d68e377e1e3f201dcc9db5e4db236b185c97f593d9685e`  
		Last Modified: Tue, 04 Jul 2023 23:50:46 GMT  
		Size: 18.6 MB (18598537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71eecde55db05e6ff5b4e60e55dbd1384f71e3c2d4256a02804eaf7348f1c6f6`  
		Last Modified: Tue, 04 Jul 2023 23:50:44 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb05d1e3693bac15fa4b4278eca59528e675f55de77bda988bb25ceab35206dd`  
		Last Modified: Tue, 04 Jul 2023 23:51:17 GMT  
		Size: 48.8 MB (48752687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d951f91bfb3b996e0fbfd7cc299a5330ba2f9e43ae268d3d04e0c6eba7257cf`  
		Last Modified: Tue, 04 Jul 2023 23:51:11 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
