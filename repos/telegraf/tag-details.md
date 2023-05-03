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
-	[`telegraf:1.26.2`](#telegraf1262)
-	[`telegraf:1.26.2-alpine`](#telegraf1262-alpine)
-	[`telegraf:alpine`](#telegrafalpine)
-	[`telegraf:latest`](#telegraflatest)

## `telegraf:1.24`

```console
$ docker pull telegraf@sha256:c70b806d6882713d2d31fa4ea1cc28fe14cbae1119005980a4a18c69b6f2487c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.24` - linux; amd64

```console
$ docker pull telegraf@sha256:5649203810334e4784241d83a98bcabe5c2d53fe349f218f717e483a8f60d41e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.4 MB (134410323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f29ffac47c9aa352c7e56b250fd381f1bcd9a329542bb38a998d860e3a93c16`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:12:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:46:36 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:46:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 19:46:38 GMT
ENV TELEGRAF_VERSION=1.24.4
# Wed, 03 May 2023 19:46:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 19:46:41 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 May 2023 19:46:41 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 May 2023 19:46:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 19:46:42 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120eb239658edf0b32a0e7e017916cc0f4cd2b167667609f87d597547b618def`  
		Last Modified: Tue, 02 May 2023 23:38:51 GMT  
		Size: 16.1 MB (16127919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f9025f8d4ab0e75729b0b4670f8d358bff16e1e5bf2d70553dbc4dec10ec0f`  
		Last Modified: Wed, 03 May 2023 19:47:15 GMT  
		Size: 18.8 MB (18760087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b631b8fdc1c1b0862e3776883eaa75478dce42107a3f2379ddc3d262d8c9dfd0`  
		Last Modified: Wed, 03 May 2023 19:47:11 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ecc72f9135ec73bee11604ff0b085daeb24c5c18205bdb82e62850d25403c7`  
		Last Modified: Wed, 03 May 2023 19:47:18 GMT  
		Size: 44.5 MB (44467441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d1c2545844d4e3b8521f2cf39dfb462fe30de34b0224e5f12a31292ee8baa6`  
		Last Modified: Wed, 03 May 2023 19:47:11 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.24` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:ba58ec574ee349107d2db4293e0388cc43524d4c11041a8ff22adaaace1b5d26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124413845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06b9609233576298edd9e67743fb523b1f1d7d93045112d6fe9197c30717be47`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:35 GMT
ADD file:75c57df33c95251a80549b7949853df282a42bc4e5f19176764907a54b74caa9 in / 
# Tue, 11 Apr 2023 23:59:36 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:00:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 15:46:22 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 15:46:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 15:46:23 GMT
ENV TELEGRAF_VERSION=1.24.4
# Wed, 03 May 2023 15:46:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 15:46:33 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 May 2023 15:46:34 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 May 2023 15:46:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 15:46:34 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4feff9b88735325634445419eaaec2ed47500b63027cfd2de34b8bc6d55ee85c`  
		Last Modified: Wed, 12 Apr 2023 00:02:57 GMT  
		Size: 50.2 MB (50216882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6db5edf7d5760b7d208f139af10d322cde628cc8c3701f8c2088c02ab63ec10`  
		Last Modified: Tue, 02 May 2023 23:35:39 GMT  
		Size: 15.2 MB (15225182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ff7ae6579de96f50e474855d6614d2a0193ca2808fe137f3db1b7ef6d31812`  
		Last Modified: Wed, 03 May 2023 15:47:05 GMT  
		Size: 17.5 MB (17462486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0516e36d06ad16cd2f8646ea401fda7e286cf83be2112a4ee3494b69a90569a0`  
		Last Modified: Wed, 03 May 2023 15:47:02 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105f60b9c5d1234935ac8d4b17fdb4cc8dc0013d44f5cc74d8dfc8556883e76a`  
		Last Modified: Wed, 03 May 2023 15:47:09 GMT  
		Size: 41.5 MB (41507143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cffb0162e8f20e4b32eb371d5b9a69479932072cfa7f6b132fffdd8e7d31086`  
		Last Modified: Wed, 03 May 2023 15:47:02 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.24` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:ee6e504687cae7997c080a332258bfe8073a37f351511e606eada3561329bd32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128722824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2773bdb561feb443a077ea58456d06c1a60b3f1bbc1d88fb1c14bb2d4696dc1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:41:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 12:03:52 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 12:03:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 12:03:53 GMT
ENV TELEGRAF_VERSION=1.24.4
# Wed, 03 May 2023 12:03:56 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 12:03:57 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 May 2023 12:03:57 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 May 2023 12:03:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 12:03:57 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5399ff5f54e66385506fb32e1b1ccf2d1bbe3a61b951f9b03e667cd68dfe58f`  
		Last Modified: Wed, 03 May 2023 00:11:16 GMT  
		Size: 16.1 MB (16111036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cac6cbaa7c4f26b22c1a1ed949789e02ef047f62ca9afa5b4c8d528f1c0222`  
		Last Modified: Wed, 03 May 2023 12:04:25 GMT  
		Size: 18.6 MB (18598598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3150c2c3bf48d024506124f22deaf52710818ce1b5b989ce1b429c517befdd0b`  
		Last Modified: Wed, 03 May 2023 12:04:22 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92be811c775b21a5361c944cc617e223d2152435248677b6cda570b10d4b0a4`  
		Last Modified: Wed, 03 May 2023 12:04:27 GMT  
		Size: 40.3 MB (40305512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328f65c439d65f4bc5a8e782ce9330a46023bdc8fbf54b505e2ea0209cdbda62`  
		Last Modified: Wed, 03 May 2023 12:04:22 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.24-alpine`

```console
$ docker pull telegraf@sha256:b2c7b7b4357f0a941013b6814745c3554b8576ba745723d1bc0b9b26bd5bdddf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.24-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:ccddf3aae06c6a7fa5e7ba6f5609fb79530c72c2435be98192cb4de5150adc7e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50340376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a75343f85a824d5dca55965f1ea4ea791a54dd7b67dee84d8ef0e7f3ce1c9d9`
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
# Thu, 30 Mar 2023 02:39:58 GMT
ENV TELEGRAF_VERSION=1.24.4
# Thu, 30 Mar 2023 02:40:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Thu, 30 Mar 2023 02:40:05 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 30 Mar 2023 02:40:05 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Thu, 30 Mar 2023 02:40:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 02:40:06 GMT
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
	-	`sha256:4838940349ebcf9f5ebe89e7fea69ced09c8aff2bb7b4938d8b1d44f4d7ae811`  
		Last Modified: Thu, 30 Mar 2023 02:40:45 GMT  
		Size: 44.3 MB (44293897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4c64c062f591ac9a818712808e81d4a81e5e41a935edc17d0a0c63dce41dd0`  
		Last Modified: Thu, 30 Mar 2023 02:40:38 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.24.4`

```console
$ docker pull telegraf@sha256:c70b806d6882713d2d31fa4ea1cc28fe14cbae1119005980a4a18c69b6f2487c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.24.4` - linux; amd64

```console
$ docker pull telegraf@sha256:5649203810334e4784241d83a98bcabe5c2d53fe349f218f717e483a8f60d41e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.4 MB (134410323 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f29ffac47c9aa352c7e56b250fd381f1bcd9a329542bb38a998d860e3a93c16`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:12:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:46:36 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:46:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 19:46:38 GMT
ENV TELEGRAF_VERSION=1.24.4
# Wed, 03 May 2023 19:46:41 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 19:46:41 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 May 2023 19:46:41 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 May 2023 19:46:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 19:46:42 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120eb239658edf0b32a0e7e017916cc0f4cd2b167667609f87d597547b618def`  
		Last Modified: Tue, 02 May 2023 23:38:51 GMT  
		Size: 16.1 MB (16127919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f9025f8d4ab0e75729b0b4670f8d358bff16e1e5bf2d70553dbc4dec10ec0f`  
		Last Modified: Wed, 03 May 2023 19:47:15 GMT  
		Size: 18.8 MB (18760087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b631b8fdc1c1b0862e3776883eaa75478dce42107a3f2379ddc3d262d8c9dfd0`  
		Last Modified: Wed, 03 May 2023 19:47:11 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ecc72f9135ec73bee11604ff0b085daeb24c5c18205bdb82e62850d25403c7`  
		Last Modified: Wed, 03 May 2023 19:47:18 GMT  
		Size: 44.5 MB (44467441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3d1c2545844d4e3b8521f2cf39dfb462fe30de34b0224e5f12a31292ee8baa6`  
		Last Modified: Wed, 03 May 2023 19:47:11 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.24.4` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:ba58ec574ee349107d2db4293e0388cc43524d4c11041a8ff22adaaace1b5d26
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.4 MB (124413845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06b9609233576298edd9e67743fb523b1f1d7d93045112d6fe9197c30717be47`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:35 GMT
ADD file:75c57df33c95251a80549b7949853df282a42bc4e5f19176764907a54b74caa9 in / 
# Tue, 11 Apr 2023 23:59:36 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:00:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 15:46:22 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 15:46:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 15:46:23 GMT
ENV TELEGRAF_VERSION=1.24.4
# Wed, 03 May 2023 15:46:33 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 15:46:33 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 May 2023 15:46:34 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 May 2023 15:46:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 15:46:34 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4feff9b88735325634445419eaaec2ed47500b63027cfd2de34b8bc6d55ee85c`  
		Last Modified: Wed, 12 Apr 2023 00:02:57 GMT  
		Size: 50.2 MB (50216882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6db5edf7d5760b7d208f139af10d322cde628cc8c3701f8c2088c02ab63ec10`  
		Last Modified: Tue, 02 May 2023 23:35:39 GMT  
		Size: 15.2 MB (15225182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ff7ae6579de96f50e474855d6614d2a0193ca2808fe137f3db1b7ef6d31812`  
		Last Modified: Wed, 03 May 2023 15:47:05 GMT  
		Size: 17.5 MB (17462486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0516e36d06ad16cd2f8646ea401fda7e286cf83be2112a4ee3494b69a90569a0`  
		Last Modified: Wed, 03 May 2023 15:47:02 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105f60b9c5d1234935ac8d4b17fdb4cc8dc0013d44f5cc74d8dfc8556883e76a`  
		Last Modified: Wed, 03 May 2023 15:47:09 GMT  
		Size: 41.5 MB (41507143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cffb0162e8f20e4b32eb371d5b9a69479932072cfa7f6b132fffdd8e7d31086`  
		Last Modified: Wed, 03 May 2023 15:47:02 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.24.4` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:ee6e504687cae7997c080a332258bfe8073a37f351511e606eada3561329bd32
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.7 MB (128722824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2773bdb561feb443a077ea58456d06c1a60b3f1bbc1d88fb1c14bb2d4696dc1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:41:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 12:03:52 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 12:03:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 12:03:53 GMT
ENV TELEGRAF_VERSION=1.24.4
# Wed, 03 May 2023 12:03:56 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 12:03:57 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 May 2023 12:03:57 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 May 2023 12:03:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 12:03:57 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5399ff5f54e66385506fb32e1b1ccf2d1bbe3a61b951f9b03e667cd68dfe58f`  
		Last Modified: Wed, 03 May 2023 00:11:16 GMT  
		Size: 16.1 MB (16111036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cac6cbaa7c4f26b22c1a1ed949789e02ef047f62ca9afa5b4c8d528f1c0222`  
		Last Modified: Wed, 03 May 2023 12:04:25 GMT  
		Size: 18.6 MB (18598598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3150c2c3bf48d024506124f22deaf52710818ce1b5b989ce1b429c517befdd0b`  
		Last Modified: Wed, 03 May 2023 12:04:22 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92be811c775b21a5361c944cc617e223d2152435248677b6cda570b10d4b0a4`  
		Last Modified: Wed, 03 May 2023 12:04:27 GMT  
		Size: 40.3 MB (40305512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:328f65c439d65f4bc5a8e782ce9330a46023bdc8fbf54b505e2ea0209cdbda62`  
		Last Modified: Wed, 03 May 2023 12:04:22 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.24.4-alpine`

```console
$ docker pull telegraf@sha256:b2c7b7b4357f0a941013b6814745c3554b8576ba745723d1bc0b9b26bd5bdddf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:1.24.4-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:ccddf3aae06c6a7fa5e7ba6f5609fb79530c72c2435be98192cb4de5150adc7e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50340376 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a75343f85a824d5dca55965f1ea4ea791a54dd7b67dee84d8ef0e7f3ce1c9d9`
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
# Thu, 30 Mar 2023 02:39:58 GMT
ENV TELEGRAF_VERSION=1.24.4
# Thu, 30 Mar 2023 02:40:05 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Thu, 30 Mar 2023 02:40:05 GMT
EXPOSE 8092/udp 8094 8125/udp
# Thu, 30 Mar 2023 02:40:05 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Thu, 30 Mar 2023 02:40:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 30 Mar 2023 02:40:06 GMT
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
	-	`sha256:4838940349ebcf9f5ebe89e7fea69ced09c8aff2bb7b4938d8b1d44f4d7ae811`  
		Last Modified: Thu, 30 Mar 2023 02:40:45 GMT  
		Size: 44.3 MB (44293897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4c64c062f591ac9a818712808e81d4a81e5e41a935edc17d0a0c63dce41dd0`  
		Last Modified: Thu, 30 Mar 2023 02:40:38 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.25`

```console
$ docker pull telegraf@sha256:6668144cc0c5ca9b33814aa9af32def79e3654f8112eb7b60ec37a1b94e02a60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.25` - linux; amd64

```console
$ docker pull telegraf@sha256:5efce0123a67f706b51f001792e4a6cb2527d2635d7540ad2349c243641ce93c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.5 MB (136519562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6480312aee525f4c4d592b5958e163a9d17cc05221767c5f36019845e5900e3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:12:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:46:36 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:46:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 19:46:47 GMT
ENV TELEGRAF_VERSION=1.25.3
# Wed, 03 May 2023 19:46:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 19:46:50 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 May 2023 19:46:50 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 May 2023 19:46:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 19:46:51 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120eb239658edf0b32a0e7e017916cc0f4cd2b167667609f87d597547b618def`  
		Last Modified: Tue, 02 May 2023 23:38:51 GMT  
		Size: 16.1 MB (16127919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f9025f8d4ab0e75729b0b4670f8d358bff16e1e5bf2d70553dbc4dec10ec0f`  
		Last Modified: Wed, 03 May 2023 19:47:15 GMT  
		Size: 18.8 MB (18760087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b631b8fdc1c1b0862e3776883eaa75478dce42107a3f2379ddc3d262d8c9dfd0`  
		Last Modified: Wed, 03 May 2023 19:47:11 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeae665e273bcbde5a9e794a5e21f65519398ba504229030b466fee9c158944`  
		Last Modified: Wed, 03 May 2023 19:47:34 GMT  
		Size: 46.6 MB (46576681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0391dd5697a7495dc9f7b73178e7f14ad0833bc825b9ab0f856a1f474134155`  
		Last Modified: Wed, 03 May 2023 19:47:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:df2d76dce8c38e26d5df22d10dc861c343b1774e0309d1fb7a021632f80b5d0b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.3 MB (126290686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34659e40437f23ae843bfde9bad508ecc60a0305c390cf611132d5eb158c5b7d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:35 GMT
ADD file:75c57df33c95251a80549b7949853df282a42bc4e5f19176764907a54b74caa9 in / 
# Tue, 11 Apr 2023 23:59:36 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:00:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 15:46:22 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 15:46:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 15:46:36 GMT
ENV TELEGRAF_VERSION=1.25.3
# Wed, 03 May 2023 15:46:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 15:46:43 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 May 2023 15:46:43 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 May 2023 15:46:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 15:46:43 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4feff9b88735325634445419eaaec2ed47500b63027cfd2de34b8bc6d55ee85c`  
		Last Modified: Wed, 12 Apr 2023 00:02:57 GMT  
		Size: 50.2 MB (50216882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6db5edf7d5760b7d208f139af10d322cde628cc8c3701f8c2088c02ab63ec10`  
		Last Modified: Tue, 02 May 2023 23:35:39 GMT  
		Size: 15.2 MB (15225182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ff7ae6579de96f50e474855d6614d2a0193ca2808fe137f3db1b7ef6d31812`  
		Last Modified: Wed, 03 May 2023 15:47:05 GMT  
		Size: 17.5 MB (17462486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0516e36d06ad16cd2f8646ea401fda7e286cf83be2112a4ee3494b69a90569a0`  
		Last Modified: Wed, 03 May 2023 15:47:02 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd536dd8938e9cba028b8a2ef2c0c3c15c81e73f0fa4d31b5f8a812983b9f971`  
		Last Modified: Wed, 03 May 2023 15:47:24 GMT  
		Size: 43.4 MB (43383983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9617e0f8dcb19508907c00f83175c926cc2e2a311727cc5a3ff8a3d9d3c035`  
		Last Modified: Wed, 03 May 2023 15:47:17 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:e3ff8935ac590fcc20e5e574f77002cb0375e9f5e12d80d7aaa766c3fe0ca939
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130732590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ff1650be19c8c72725db52880b19656b8076be2220b822c8d2e9b06099caa71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:41:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 12:03:52 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 12:03:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 12:03:59 GMT
ENV TELEGRAF_VERSION=1.25.3
# Wed, 03 May 2023 12:04:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 12:04:04 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 May 2023 12:04:04 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 May 2023 12:04:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 12:04:04 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5399ff5f54e66385506fb32e1b1ccf2d1bbe3a61b951f9b03e667cd68dfe58f`  
		Last Modified: Wed, 03 May 2023 00:11:16 GMT  
		Size: 16.1 MB (16111036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cac6cbaa7c4f26b22c1a1ed949789e02ef047f62ca9afa5b4c8d528f1c0222`  
		Last Modified: Wed, 03 May 2023 12:04:25 GMT  
		Size: 18.6 MB (18598598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3150c2c3bf48d024506124f22deaf52710818ce1b5b989ce1b429c517befdd0b`  
		Last Modified: Wed, 03 May 2023 12:04:22 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24eda3ef0e0214027db2fd97fc8396fa133d656dbecbe983f80307277befcb0a`  
		Last Modified: Wed, 03 May 2023 12:04:40 GMT  
		Size: 42.3 MB (42315277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9508679f82e48b082121cbba58264f93ee590f14dac07dd728888a76784dbfb`  
		Last Modified: Wed, 03 May 2023 12:04:35 GMT  
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
$ docker pull telegraf@sha256:6668144cc0c5ca9b33814aa9af32def79e3654f8112eb7b60ec37a1b94e02a60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.25.3` - linux; amd64

```console
$ docker pull telegraf@sha256:5efce0123a67f706b51f001792e4a6cb2527d2635d7540ad2349c243641ce93c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.5 MB (136519562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6480312aee525f4c4d592b5958e163a9d17cc05221767c5f36019845e5900e3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:12:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:46:36 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:46:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 19:46:47 GMT
ENV TELEGRAF_VERSION=1.25.3
# Wed, 03 May 2023 19:46:50 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 19:46:50 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 May 2023 19:46:50 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 May 2023 19:46:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 19:46:51 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120eb239658edf0b32a0e7e017916cc0f4cd2b167667609f87d597547b618def`  
		Last Modified: Tue, 02 May 2023 23:38:51 GMT  
		Size: 16.1 MB (16127919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f9025f8d4ab0e75729b0b4670f8d358bff16e1e5bf2d70553dbc4dec10ec0f`  
		Last Modified: Wed, 03 May 2023 19:47:15 GMT  
		Size: 18.8 MB (18760087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b631b8fdc1c1b0862e3776883eaa75478dce42107a3f2379ddc3d262d8c9dfd0`  
		Last Modified: Wed, 03 May 2023 19:47:11 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffeae665e273bcbde5a9e794a5e21f65519398ba504229030b466fee9c158944`  
		Last Modified: Wed, 03 May 2023 19:47:34 GMT  
		Size: 46.6 MB (46576681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0391dd5697a7495dc9f7b73178e7f14ad0833bc825b9ab0f856a1f474134155`  
		Last Modified: Wed, 03 May 2023 19:47:27 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25.3` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:df2d76dce8c38e26d5df22d10dc861c343b1774e0309d1fb7a021632f80b5d0b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.3 MB (126290686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34659e40437f23ae843bfde9bad508ecc60a0305c390cf611132d5eb158c5b7d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:35 GMT
ADD file:75c57df33c95251a80549b7949853df282a42bc4e5f19176764907a54b74caa9 in / 
# Tue, 11 Apr 2023 23:59:36 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:00:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 15:46:22 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 15:46:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 15:46:36 GMT
ENV TELEGRAF_VERSION=1.25.3
# Wed, 03 May 2023 15:46:42 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 15:46:43 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 May 2023 15:46:43 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 May 2023 15:46:43 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 15:46:43 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4feff9b88735325634445419eaaec2ed47500b63027cfd2de34b8bc6d55ee85c`  
		Last Modified: Wed, 12 Apr 2023 00:02:57 GMT  
		Size: 50.2 MB (50216882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6db5edf7d5760b7d208f139af10d322cde628cc8c3701f8c2088c02ab63ec10`  
		Last Modified: Tue, 02 May 2023 23:35:39 GMT  
		Size: 15.2 MB (15225182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ff7ae6579de96f50e474855d6614d2a0193ca2808fe137f3db1b7ef6d31812`  
		Last Modified: Wed, 03 May 2023 15:47:05 GMT  
		Size: 17.5 MB (17462486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0516e36d06ad16cd2f8646ea401fda7e286cf83be2112a4ee3494b69a90569a0`  
		Last Modified: Wed, 03 May 2023 15:47:02 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd536dd8938e9cba028b8a2ef2c0c3c15c81e73f0fa4d31b5f8a812983b9f971`  
		Last Modified: Wed, 03 May 2023 15:47:24 GMT  
		Size: 43.4 MB (43383983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9617e0f8dcb19508907c00f83175c926cc2e2a311727cc5a3ff8a3d9d3c035`  
		Last Modified: Wed, 03 May 2023 15:47:17 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.25.3` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:e3ff8935ac590fcc20e5e574f77002cb0375e9f5e12d80d7aaa766c3fe0ca939
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130732590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ff1650be19c8c72725db52880b19656b8076be2220b822c8d2e9b06099caa71`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:41:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 12:03:52 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 12:03:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 12:03:59 GMT
ENV TELEGRAF_VERSION=1.25.3
# Wed, 03 May 2023 12:04:03 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 12:04:04 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 May 2023 12:04:04 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 May 2023 12:04:04 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 12:04:04 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5399ff5f54e66385506fb32e1b1ccf2d1bbe3a61b951f9b03e667cd68dfe58f`  
		Last Modified: Wed, 03 May 2023 00:11:16 GMT  
		Size: 16.1 MB (16111036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cac6cbaa7c4f26b22c1a1ed949789e02ef047f62ca9afa5b4c8d528f1c0222`  
		Last Modified: Wed, 03 May 2023 12:04:25 GMT  
		Size: 18.6 MB (18598598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3150c2c3bf48d024506124f22deaf52710818ce1b5b989ce1b429c517befdd0b`  
		Last Modified: Wed, 03 May 2023 12:04:22 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24eda3ef0e0214027db2fd97fc8396fa133d656dbecbe983f80307277befcb0a`  
		Last Modified: Wed, 03 May 2023 12:04:40 GMT  
		Size: 42.3 MB (42315277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9508679f82e48b082121cbba58264f93ee590f14dac07dd728888a76784dbfb`  
		Last Modified: Wed, 03 May 2023 12:04:35 GMT  
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
$ docker pull telegraf@sha256:07f352362b74a7ef05d6ebcdd73ebc9b4bdb7d22860942acebd786a857f131c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.26` - linux; amd64

```console
$ docker pull telegraf@sha256:21aa5b8ed090a333aa55ff0e8d16c1fbdc7ba65fabaf4edbbc07c71b59494928
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137875647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44a6417f9d736f81e6d0d34e5041f843de0a2e4b591e3f4e901e741ddf8fb261`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:12:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:46:36 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:46:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 19:46:54 GMT
ENV TELEGRAF_VERSION=1.26.2
# Wed, 03 May 2023 19:46:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 19:46:58 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 May 2023 19:46:58 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 May 2023 19:46:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 19:46:58 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120eb239658edf0b32a0e7e017916cc0f4cd2b167667609f87d597547b618def`  
		Last Modified: Tue, 02 May 2023 23:38:51 GMT  
		Size: 16.1 MB (16127919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f9025f8d4ab0e75729b0b4670f8d358bff16e1e5bf2d70553dbc4dec10ec0f`  
		Last Modified: Wed, 03 May 2023 19:47:15 GMT  
		Size: 18.8 MB (18760087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b631b8fdc1c1b0862e3776883eaa75478dce42107a3f2379ddc3d262d8c9dfd0`  
		Last Modified: Wed, 03 May 2023 19:47:11 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5effc481dfc0f5e4ba246bf26fbac8c74da64e9aa7d46e3a5200c9e56f3ebe77`  
		Last Modified: Wed, 03 May 2023 19:47:50 GMT  
		Size: 47.9 MB (47932766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc2e1f7d5b4385daa362bef293742964568b5f93f99b412cc1547565f68972f`  
		Last Modified: Wed, 03 May 2023 19:47:43 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:e0f232ae5a7e8c2c0fa2fad719bcb098711d9d4ad62f4b13474417fe824bc999
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.6 MB (127604546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6fe87652aa184a1bdab9b2f895ff60572f87e48ff725b03d13441a5b7799d0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:35 GMT
ADD file:75c57df33c95251a80549b7949853df282a42bc4e5f19176764907a54b74caa9 in / 
# Tue, 11 Apr 2023 23:59:36 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:00:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 15:46:22 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 15:46:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 15:46:46 GMT
ENV TELEGRAF_VERSION=1.26.2
# Wed, 03 May 2023 15:46:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 15:46:52 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 May 2023 15:46:52 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 May 2023 15:46:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 15:46:52 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4feff9b88735325634445419eaaec2ed47500b63027cfd2de34b8bc6d55ee85c`  
		Last Modified: Wed, 12 Apr 2023 00:02:57 GMT  
		Size: 50.2 MB (50216882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6db5edf7d5760b7d208f139af10d322cde628cc8c3701f8c2088c02ab63ec10`  
		Last Modified: Tue, 02 May 2023 23:35:39 GMT  
		Size: 15.2 MB (15225182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ff7ae6579de96f50e474855d6614d2a0193ca2808fe137f3db1b7ef6d31812`  
		Last Modified: Wed, 03 May 2023 15:47:05 GMT  
		Size: 17.5 MB (17462486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0516e36d06ad16cd2f8646ea401fda7e286cf83be2112a4ee3494b69a90569a0`  
		Last Modified: Wed, 03 May 2023 15:47:02 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ac155059d8232658760b0656227ce019ad0c26756fbc7625036855ae7f430c`  
		Last Modified: Wed, 03 May 2023 15:47:41 GMT  
		Size: 44.7 MB (44697847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92a5d0f8244e1b6af8a581f61717f1df117db446c6686e31ca7e36706671898`  
		Last Modified: Wed, 03 May 2023 15:47:32 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:283635aa4c19871f7bba4a69bc2bc1b120137e4bcfad6e03367742645382c330
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.0 MB (132025942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00831f62ce55307a6e81c8dcd1c5df90024f91b6ed0613dd810d09e2ce1b06cd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:41:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 12:03:52 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 12:03:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 12:04:06 GMT
ENV TELEGRAF_VERSION=1.26.2
# Wed, 03 May 2023 12:04:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 12:04:10 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 May 2023 12:04:10 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 May 2023 12:04:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 12:04:10 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5399ff5f54e66385506fb32e1b1ccf2d1bbe3a61b951f9b03e667cd68dfe58f`  
		Last Modified: Wed, 03 May 2023 00:11:16 GMT  
		Size: 16.1 MB (16111036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cac6cbaa7c4f26b22c1a1ed949789e02ef047f62ca9afa5b4c8d528f1c0222`  
		Last Modified: Wed, 03 May 2023 12:04:25 GMT  
		Size: 18.6 MB (18598598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3150c2c3bf48d024506124f22deaf52710818ce1b5b989ce1b429c517befdd0b`  
		Last Modified: Wed, 03 May 2023 12:04:22 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ac80241bed019de8ae31d8037681a48718c04c105f8a35931734a8ac037a20`  
		Last Modified: Wed, 03 May 2023 12:04:52 GMT  
		Size: 43.6 MB (43608627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1218ee010e969e454e992fcf4f3f3b4d192f20aa5140b7afd477fa35fced2ba8`  
		Last Modified: Wed, 03 May 2023 12:04:47 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26-alpine`

```console
$ docker pull telegraf@sha256:f408e385670a4c98ac0f9e9588c2ffaa7c7f194abab6556aa19830d7085a1223
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.26-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:8f44f38e4fab836d5815753a22866128019a47fc4e624a4b0767d411aaf320b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53821481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b2b8ed0578f280e0022d43dbd9f4e59504dc44ff6880c2515a69aefab21e661`
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
# Mon, 24 Apr 2023 20:19:06 GMT
ENV TELEGRAF_VERSION=1.26.2
# Mon, 24 Apr 2023 20:19:12 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 24 Apr 2023 20:19:12 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 24 Apr 2023 20:19:12 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 24 Apr 2023 20:19:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Apr 2023 20:19:13 GMT
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
	-	`sha256:e5bd32666a1f4d04b3cb13ea24c39fb9a787d89385e3a11637c93a48fcdeadb2`  
		Last Modified: Mon, 24 Apr 2023 20:19:52 GMT  
		Size: 47.8 MB (47775002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dccc1c8e69b38525461e950b504b8f639d57d6f7c5751d781dfaef711573499d`  
		Last Modified: Mon, 24 Apr 2023 20:19:44 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:18054e4e199d2f0d212682b2d64aaeda2fac97d97af7911a5df6654bc0d656f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49408782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:678399f6c28da2a7ff3bf6c34dd0a81ef45f4201f510f593176db0e1941e07b1`
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
# Mon, 24 Apr 2023 20:03:23 GMT
ENV TELEGRAF_VERSION=1.26.2
# Mon, 24 Apr 2023 20:03:29 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 24 Apr 2023 20:03:30 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 24 Apr 2023 20:03:30 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 24 Apr 2023 20:03:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Apr 2023 20:03:30 GMT
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
	-	`sha256:e079ae89d80ef01555b2edb2bce1493944785cbb674324fc8001fd5c3c56581f`  
		Last Modified: Mon, 24 Apr 2023 20:04:06 GMT  
		Size: 43.4 MB (43442990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4261ed7b7c080fc61dfde80adfe1097df13d9327a72179e208d7f7851f500c0f`  
		Last Modified: Mon, 24 Apr 2023 20:04:01 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26.2`

```console
$ docker pull telegraf@sha256:07f352362b74a7ef05d6ebcdd73ebc9b4bdb7d22860942acebd786a857f131c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:1.26.2` - linux; amd64

```console
$ docker pull telegraf@sha256:21aa5b8ed090a333aa55ff0e8d16c1fbdc7ba65fabaf4edbbc07c71b59494928
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137875647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44a6417f9d736f81e6d0d34e5041f843de0a2e4b591e3f4e901e741ddf8fb261`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:12:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:46:36 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:46:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 19:46:54 GMT
ENV TELEGRAF_VERSION=1.26.2
# Wed, 03 May 2023 19:46:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 19:46:58 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 May 2023 19:46:58 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 May 2023 19:46:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 19:46:58 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120eb239658edf0b32a0e7e017916cc0f4cd2b167667609f87d597547b618def`  
		Last Modified: Tue, 02 May 2023 23:38:51 GMT  
		Size: 16.1 MB (16127919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f9025f8d4ab0e75729b0b4670f8d358bff16e1e5bf2d70553dbc4dec10ec0f`  
		Last Modified: Wed, 03 May 2023 19:47:15 GMT  
		Size: 18.8 MB (18760087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b631b8fdc1c1b0862e3776883eaa75478dce42107a3f2379ddc3d262d8c9dfd0`  
		Last Modified: Wed, 03 May 2023 19:47:11 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5effc481dfc0f5e4ba246bf26fbac8c74da64e9aa7d46e3a5200c9e56f3ebe77`  
		Last Modified: Wed, 03 May 2023 19:47:50 GMT  
		Size: 47.9 MB (47932766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc2e1f7d5b4385daa362bef293742964568b5f93f99b412cc1547565f68972f`  
		Last Modified: Wed, 03 May 2023 19:47:43 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26.2` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:e0f232ae5a7e8c2c0fa2fad719bcb098711d9d4ad62f4b13474417fe824bc999
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.6 MB (127604546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6fe87652aa184a1bdab9b2f895ff60572f87e48ff725b03d13441a5b7799d0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:35 GMT
ADD file:75c57df33c95251a80549b7949853df282a42bc4e5f19176764907a54b74caa9 in / 
# Tue, 11 Apr 2023 23:59:36 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:00:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 15:46:22 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 15:46:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 15:46:46 GMT
ENV TELEGRAF_VERSION=1.26.2
# Wed, 03 May 2023 15:46:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 15:46:52 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 May 2023 15:46:52 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 May 2023 15:46:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 15:46:52 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4feff9b88735325634445419eaaec2ed47500b63027cfd2de34b8bc6d55ee85c`  
		Last Modified: Wed, 12 Apr 2023 00:02:57 GMT  
		Size: 50.2 MB (50216882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6db5edf7d5760b7d208f139af10d322cde628cc8c3701f8c2088c02ab63ec10`  
		Last Modified: Tue, 02 May 2023 23:35:39 GMT  
		Size: 15.2 MB (15225182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ff7ae6579de96f50e474855d6614d2a0193ca2808fe137f3db1b7ef6d31812`  
		Last Modified: Wed, 03 May 2023 15:47:05 GMT  
		Size: 17.5 MB (17462486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0516e36d06ad16cd2f8646ea401fda7e286cf83be2112a4ee3494b69a90569a0`  
		Last Modified: Wed, 03 May 2023 15:47:02 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ac155059d8232658760b0656227ce019ad0c26756fbc7625036855ae7f430c`  
		Last Modified: Wed, 03 May 2023 15:47:41 GMT  
		Size: 44.7 MB (44697847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92a5d0f8244e1b6af8a581f61717f1df117db446c6686e31ca7e36706671898`  
		Last Modified: Wed, 03 May 2023 15:47:32 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26.2` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:283635aa4c19871f7bba4a69bc2bc1b120137e4bcfad6e03367742645382c330
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.0 MB (132025942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00831f62ce55307a6e81c8dcd1c5df90024f91b6ed0613dd810d09e2ce1b06cd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:41:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 12:03:52 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 12:03:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 12:04:06 GMT
ENV TELEGRAF_VERSION=1.26.2
# Wed, 03 May 2023 12:04:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 12:04:10 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 May 2023 12:04:10 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 May 2023 12:04:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 12:04:10 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5399ff5f54e66385506fb32e1b1ccf2d1bbe3a61b951f9b03e667cd68dfe58f`  
		Last Modified: Wed, 03 May 2023 00:11:16 GMT  
		Size: 16.1 MB (16111036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cac6cbaa7c4f26b22c1a1ed949789e02ef047f62ca9afa5b4c8d528f1c0222`  
		Last Modified: Wed, 03 May 2023 12:04:25 GMT  
		Size: 18.6 MB (18598598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3150c2c3bf48d024506124f22deaf52710818ce1b5b989ce1b429c517befdd0b`  
		Last Modified: Wed, 03 May 2023 12:04:22 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ac80241bed019de8ae31d8037681a48718c04c105f8a35931734a8ac037a20`  
		Last Modified: Wed, 03 May 2023 12:04:52 GMT  
		Size: 43.6 MB (43608627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1218ee010e969e454e992fcf4f3f3b4d192f20aa5140b7afd477fa35fced2ba8`  
		Last Modified: Wed, 03 May 2023 12:04:47 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:1.26.2-alpine`

```console
$ docker pull telegraf@sha256:f408e385670a4c98ac0f9e9588c2ffaa7c7f194abab6556aa19830d7085a1223
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:1.26.2-alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:8f44f38e4fab836d5815753a22866128019a47fc4e624a4b0767d411aaf320b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53821481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b2b8ed0578f280e0022d43dbd9f4e59504dc44ff6880c2515a69aefab21e661`
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
# Mon, 24 Apr 2023 20:19:06 GMT
ENV TELEGRAF_VERSION=1.26.2
# Mon, 24 Apr 2023 20:19:12 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 24 Apr 2023 20:19:12 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 24 Apr 2023 20:19:12 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 24 Apr 2023 20:19:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Apr 2023 20:19:13 GMT
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
	-	`sha256:e5bd32666a1f4d04b3cb13ea24c39fb9a787d89385e3a11637c93a48fcdeadb2`  
		Last Modified: Mon, 24 Apr 2023 20:19:52 GMT  
		Size: 47.8 MB (47775002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dccc1c8e69b38525461e950b504b8f639d57d6f7c5751d781dfaef711573499d`  
		Last Modified: Mon, 24 Apr 2023 20:19:44 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:1.26.2-alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:18054e4e199d2f0d212682b2d64aaeda2fac97d97af7911a5df6654bc0d656f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49408782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:678399f6c28da2a7ff3bf6c34dd0a81ef45f4201f510f593176db0e1941e07b1`
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
# Mon, 24 Apr 2023 20:03:23 GMT
ENV TELEGRAF_VERSION=1.26.2
# Mon, 24 Apr 2023 20:03:29 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 24 Apr 2023 20:03:30 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 24 Apr 2023 20:03:30 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 24 Apr 2023 20:03:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Apr 2023 20:03:30 GMT
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
	-	`sha256:e079ae89d80ef01555b2edb2bce1493944785cbb674324fc8001fd5c3c56581f`  
		Last Modified: Mon, 24 Apr 2023 20:04:06 GMT  
		Size: 43.4 MB (43442990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4261ed7b7c080fc61dfde80adfe1097df13d9327a72179e208d7f7851f500c0f`  
		Last Modified: Mon, 24 Apr 2023 20:04:01 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:f408e385670a4c98ac0f9e9588c2ffaa7c7f194abab6556aa19830d7085a1223
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:8f44f38e4fab836d5815753a22866128019a47fc4e624a4b0767d411aaf320b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53821481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b2b8ed0578f280e0022d43dbd9f4e59504dc44ff6880c2515a69aefab21e661`
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
# Mon, 24 Apr 2023 20:19:06 GMT
ENV TELEGRAF_VERSION=1.26.2
# Mon, 24 Apr 2023 20:19:12 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 24 Apr 2023 20:19:12 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 24 Apr 2023 20:19:12 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 24 Apr 2023 20:19:12 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Apr 2023 20:19:13 GMT
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
	-	`sha256:e5bd32666a1f4d04b3cb13ea24c39fb9a787d89385e3a11637c93a48fcdeadb2`  
		Last Modified: Mon, 24 Apr 2023 20:19:52 GMT  
		Size: 47.8 MB (47775002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dccc1c8e69b38525461e950b504b8f639d57d6f7c5751d781dfaef711573499d`  
		Last Modified: Mon, 24 Apr 2023 20:19:44 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:18054e4e199d2f0d212682b2d64aaeda2fac97d97af7911a5df6654bc0d656f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49408782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:678399f6c28da2a7ff3bf6c34dd0a81ef45f4201f510f593176db0e1941e07b1`
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
# Mon, 24 Apr 2023 20:03:23 GMT
ENV TELEGRAF_VERSION=1.26.2
# Mon, 24 Apr 2023 20:03:29 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Mon, 24 Apr 2023 20:03:30 GMT
EXPOSE 8092/udp 8094 8125/udp
# Mon, 24 Apr 2023 20:03:30 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Mon, 24 Apr 2023 20:03:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Apr 2023 20:03:30 GMT
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
	-	`sha256:e079ae89d80ef01555b2edb2bce1493944785cbb674324fc8001fd5c3c56581f`  
		Last Modified: Mon, 24 Apr 2023 20:04:06 GMT  
		Size: 43.4 MB (43442990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4261ed7b7c080fc61dfde80adfe1097df13d9327a72179e208d7f7851f500c0f`  
		Last Modified: Mon, 24 Apr 2023 20:04:01 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `telegraf:latest`

```console
$ docker pull telegraf@sha256:07f352362b74a7ef05d6ebcdd73ebc9b4bdb7d22860942acebd786a857f131c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `telegraf:latest` - linux; amd64

```console
$ docker pull telegraf@sha256:21aa5b8ed090a333aa55ff0e8d16c1fbdc7ba65fabaf4edbbc07c71b59494928
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137875647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44a6417f9d736f81e6d0d34e5041f843de0a2e4b591e3f4e901e741ddf8fb261`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 12 Apr 2023 00:19:55 GMT
ADD file:f2d012660f882f319a5878a3f9ce285f488b8f90fad49ad238541cf72089e035 in / 
# Wed, 12 Apr 2023 00:19:56 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:12:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:46:36 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:46:37 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 19:46:54 GMT
ENV TELEGRAF_VERSION=1.26.2
# Wed, 03 May 2023 19:46:57 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 19:46:58 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 May 2023 19:46:58 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 May 2023 19:46:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 19:46:58 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:b0248cf3e63c73d0e496a67807d056ca41d5e968b61087e8eca2cf4b9b4d7b99`  
		Last Modified: Wed, 12 Apr 2023 00:23:20 GMT  
		Size: 55.1 MB (55052736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120eb239658edf0b32a0e7e017916cc0f4cd2b167667609f87d597547b618def`  
		Last Modified: Tue, 02 May 2023 23:38:51 GMT  
		Size: 16.1 MB (16127919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f9025f8d4ab0e75729b0b4670f8d358bff16e1e5bf2d70553dbc4dec10ec0f`  
		Last Modified: Wed, 03 May 2023 19:47:15 GMT  
		Size: 18.8 MB (18760087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b631b8fdc1c1b0862e3776883eaa75478dce42107a3f2379ddc3d262d8c9dfd0`  
		Last Modified: Wed, 03 May 2023 19:47:11 GMT  
		Size: 1.8 KB (1797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5effc481dfc0f5e4ba246bf26fbac8c74da64e9aa7d46e3a5200c9e56f3ebe77`  
		Last Modified: Wed, 03 May 2023 19:47:50 GMT  
		Size: 47.9 MB (47932766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc2e1f7d5b4385daa362bef293742964568b5f93f99b412cc1547565f68972f`  
		Last Modified: Wed, 03 May 2023 19:47:43 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm variant v7

```console
$ docker pull telegraf@sha256:e0f232ae5a7e8c2c0fa2fad719bcb098711d9d4ad62f4b13474417fe824bc999
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.6 MB (127604546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba6fe87652aa184a1bdab9b2f895ff60572f87e48ff725b03d13441a5b7799d0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Tue, 11 Apr 2023 23:59:35 GMT
ADD file:75c57df33c95251a80549b7949853df282a42bc4e5f19176764907a54b74caa9 in / 
# Tue, 11 Apr 2023 23:59:36 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:00:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 15:46:22 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 15:46:23 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 15:46:46 GMT
ENV TELEGRAF_VERSION=1.26.2
# Wed, 03 May 2023 15:46:52 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 15:46:52 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 May 2023 15:46:52 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 May 2023 15:46:52 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 15:46:52 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:4feff9b88735325634445419eaaec2ed47500b63027cfd2de34b8bc6d55ee85c`  
		Last Modified: Wed, 12 Apr 2023 00:02:57 GMT  
		Size: 50.2 MB (50216882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6db5edf7d5760b7d208f139af10d322cde628cc8c3701f8c2088c02ab63ec10`  
		Last Modified: Tue, 02 May 2023 23:35:39 GMT  
		Size: 15.2 MB (15225182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9ff7ae6579de96f50e474855d6614d2a0193ca2808fe137f3db1b7ef6d31812`  
		Last Modified: Wed, 03 May 2023 15:47:05 GMT  
		Size: 17.5 MB (17462486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0516e36d06ad16cd2f8646ea401fda7e286cf83be2112a4ee3494b69a90569a0`  
		Last Modified: Wed, 03 May 2023 15:47:02 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52ac155059d8232658760b0656227ce019ad0c26756fbc7625036855ae7f430c`  
		Last Modified: Wed, 03 May 2023 15:47:41 GMT  
		Size: 44.7 MB (44697847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92a5d0f8244e1b6af8a581f61717f1df117db446c6686e31ca7e36706671898`  
		Last Modified: Wed, 03 May 2023 15:47:32 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:latest` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:283635aa4c19871f7bba4a69bc2bc1b120137e4bcfad6e03367742645382c330
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.0 MB (132025942 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00831f62ce55307a6e81c8dcd1c5df90024f91b6ed0613dd810d09e2ce1b06cd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:42 GMT
ADD file:dd3d4e5fe819950e7d01b44a29dbd790438cd722ba76198910e2597448ab0c6f in / 
# Wed, 12 Apr 2023 00:39:43 GMT
CMD ["bash"]
# Tue, 02 May 2023 23:41:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 12:03:52 GMT
RUN DEBIAN_FRONTEND=noninteractive apt-get update &&     DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends iputils-ping snmp procps lm-sensors libcap2-bin &&     rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 12:03:53 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 03 May 2023 12:04:06 GMT
ENV TELEGRAF_VERSION=1.26.2
# Wed, 03 May 2023 12:04:09 GMT
RUN ARCH= && dpkgArch="$(dpkg --print-architecture)" &&     case "${dpkgArch##*-}" in       amd64) ARCH='amd64';;       arm64) ARCH='arm64';;       armhf) ARCH='armhf';;       armel) ARCH='armel';;       *)     echo "Unsupported architecture: ${dpkgArch}"; exit 1;;     esac &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     gpg --batch --verify telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb.asc telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     dpkg -i telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb &&     rm -f telegraf_${TELEGRAF_VERSION}-1_${ARCH}.deb*
# Wed, 03 May 2023 12:04:10 GMT
EXPOSE 8092/udp 8094 8125/udp
# Wed, 03 May 2023 12:04:10 GMT
COPY file:689e73cc90c23fa6e27f7d087886e186b6baf02bb95756b42136644d4f83a893 in /entrypoint.sh 
# Wed, 03 May 2023 12:04:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 03 May 2023 12:04:10 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:dc80b8cdbfd36cb20231d807a50d704945d1df4da8f6e23197ccfcb629970491`  
		Last Modified: Wed, 12 Apr 2023 00:42:14 GMT  
		Size: 53.7 MB (53705529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5399ff5f54e66385506fb32e1b1ccf2d1bbe3a61b951f9b03e667cd68dfe58f`  
		Last Modified: Wed, 03 May 2023 00:11:16 GMT  
		Size: 16.1 MB (16111036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cac6cbaa7c4f26b22c1a1ed949789e02ef047f62ca9afa5b4c8d528f1c0222`  
		Last Modified: Wed, 03 May 2023 12:04:25 GMT  
		Size: 18.6 MB (18598598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3150c2c3bf48d024506124f22deaf52710818ce1b5b989ce1b429c517befdd0b`  
		Last Modified: Wed, 03 May 2023 12:04:22 GMT  
		Size: 1.8 KB (1808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ac80241bed019de8ae31d8037681a48718c04c105f8a35931734a8ac037a20`  
		Last Modified: Wed, 03 May 2023 12:04:52 GMT  
		Size: 43.6 MB (43608627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1218ee010e969e454e992fcf4f3f3b4d192f20aa5140b7afd477fa35fced2ba8`  
		Last Modified: Wed, 03 May 2023 12:04:47 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
